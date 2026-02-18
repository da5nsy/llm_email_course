**Subject:** [GAIR] What you probably noticed: confidence, drift, and context

---

Week 1 of 10 - What LLMs are (and aren't)

---

If you did the tool comparison on Monday, you probably noticed something: the AI tools didn't just give different answers. They gave different answers with the same confidence. None of them said "I'm not sure about this one." None of them flagged which parts were solid and which were guesses.

That's not an accident. It's built into how these systems work.

**How LLMs generate text**

When you type a prompt, the model breaks your text into **tokens** (roughly, word fragments) and then predicts, one token at a time, what should come next. Each prediction is based on patterns learned from enormous amounts of text during training. The model isn't retrieving facts from a database. It's continuing a pattern.

Think of it like autocomplete, but operating across entire paragraphs rather than single words, drawing on patterns from billions of pages of text. The output is a plausible continuation of whatever context you've provided.

This is why the academic debate about LLMs matters for practical use. Some researchers describe them as "stochastic parrots" - sophisticated pattern matchers that remix training data without understanding. Others argue that something like reasoning emerges from next-token prediction at sufficient scale. This isn't fully settled, and both camps have evidence on their side. [TODO: Cite a recent piece from each perspective - e.g., Bender et al. for stochastic parrots, Wei et al. or similar for emergent abilities.]

What's settled, for practical purposes: the models don't know what's true. They know what sounds right. And "sounds right" is conditioned on whatever context they have - your prompt, the conversation so far, and the patterns baked in during training.

**Why context matters more than you think**

When you chat with a model, everything in the conversation window is its context. The model doesn't just respond to your last message; it responds to the entire thread. This means the conversation drifts - subtly, cumulatively - as the context grows. Early statements shape later ones. The model may start echoing your framing, reinforcing your assumptions, or gradually shifting in tone.

This is also why the same prompt can produce different results depending on what came before it. A question asked at the start of a fresh conversation and the same question asked 20 messages in can get notably different answers.

Two related things to keep in mind: models have a **knowledge cutoff** - a date beyond which their training data doesn't extend - and they reflect the biases present in their training data. We'll return to both in the coming weeks, but for now: the model's "knowledge" is a frozen snapshot of text that existed at a particular time, filtered through particular sources.

One more thing worth knowing early: models come in **open** and **closed** varieties. Closed models (like ChatGPT and Claude) run on the provider's servers - you send your data to them. Open models (like DeepSeek or Llama) can be downloaded and run locally, which matters for data privacy and for understanding what's actually inside these systems. We'll dig into this distinction in Week 8 when we talk about privacy and governance. [TODO: Update open model examples at time of sending.]

**Two ways to use a chat LLM**

There are broadly two modes. You can **generate** - give a short prompt and ask for new text (an explanation, a draft, ideas). Or you can **transform** - give it existing text and ask it to do something with that material (summarise, critique, reformat, translate).

The difference matters in practice. If you paste a methods section draft and ask for a critique, the model has your actual text and specific claims to work with. It can point to particular sentences and suggest concrete changes. If you ask it to write a methods section from scratch, it's generating based on patterns of what methods sections look like, with no grounding in your actual study. The transform mode tends to be more reliable, and we'll build on this distinction throughout the course.

## Try this: context continuation (5-8 min)

Take a paragraph you've written recently - an introduction, a methods section, an email to a collaborator. Anything where you know what comes next.

Delete the last sentence or two. Paste what remains into a chat LLM and ask: "Continue this text for one paragraph. Don't add any new factual claims beyond what's already stated."

Compare the continuation to what you actually wrote. Notice:

- Did the model match your style? Where did it miss?
- Did it sneak in new claims, even though you asked it not to?
- Did it flatten any nuance - simplify a point you'd made carefully?
- Would a reader notice the switch?

If you want to push this further, try it with two different models and compare their continuations to each other and to your original.

**Journal prompt**

Go back to your tool comparison from Monday. Now that you know more about how LLMs work - generating plausible continuations based on patterns, not looking things up - does anything about those results make more sense? Write a few lines connecting what you observed to what you've learned.
