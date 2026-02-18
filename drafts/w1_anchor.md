**Subject:** [GAIR] What you probably noticed: confidence, drift, and context

---

Week 1 of 10 - What LLMs are (and aren't)

---

If you did the tool comparison on Monday, you probably noticed something: the AI tools didn't just give different answers. They gave different answers with the same confidence. It's likely that none of them said "I'm not sure about this one." I'd bet that few of them flagged which parts were solid and which were guesses.

That's not an accident. It's built into how these systems work.

**How LLMs generate text**

When you type a prompt, the model breaks your text into **tokens** (roughly, word fragments) and then predicts, one token at a time, what should come next. Each prediction is based on patterns learned from enormous amounts of text during training. The model isn't retrieving facts from a database. It's continuing a pattern. Note that it is not doing so deterministically, always producing the same continuation. That would be boring. Instead, it picks each word out of a set of plausible options. How random that selection is determines how "creative" a model is.

Think of it like autocomplete, but operating across entire paragraphs rather than single words, drawing on patterns from billions of pages of text. The output is a plausible continuation of whatever context you've provided, generally syntactically correct, but without any guarantee of logical coherence - let alone correspondence to reality.

Whether this amounts to genuine understanding or sophisticated pattern-matching is an open debate (Christopher Summerfield's *These Strange New Minds* is a good entry point if you're curious). For our purposes, what matters is what follows from the mechanism.

**Which completion to choose?**

Not all possible continuations are created equal. Some are informative, others are not. Some use appropriate language, others regurgitate text from dark corners of the internet. So the models need to choose.

Therefore, models are trained ("fine-tuned") when it comes to the style of the answers they provide. For this, humans rate which answers they like better among sets of possible continuations, and the models are then optimised to give answers in the preferred style. Often these trainers are underpaid, rushed, and have limited expertise in the subject matter, so that answers are optimised for looking clear, confident, and charming.

This has sometimes led models to go off the deep end. Some ChatGPT versions were so sycophantic that they praised any idea users floated by them and encouraged them to commit - from the silly to the tragic that resulted in lawsuits. An early Google image model was trained to show diversity, all the way up to creating Black Nazis. This has become more balanced over time, but it is still worth remembering that the models are not optimised for truth.

They cannot be. The models don't know what's true. They know what sounds right. And "sounds right" is conditioned on whatever context they have - your prompt, the conversation so far, and the patterns baked in during training.

**Why context matters more than you think**

When you chat with a model, everything in the conversation window is its context. The model doesn't just respond to your last message; it responds to the entire thread. This means the conversation drifts - subtly, cumulatively - as the context grows. Early statements shape later ones. The model may start echoing your framing, reinforcing your assumptions, or gradually shifting in tone.

This is also why the same prompt can produce different results depending on what came before it. A question asked at the start of a fresh conversation and the same question asked 20 messages in can get notably different answers - and a question with good context about who you are and what you need tends to yield more useful results.

**Two ways to use a chat LLM**

There are broadly two modes. You can **generate** - give a short prompt and ask for new text (an explanation, a draft, ideas). Or you can **transform** - give it existing text and ask it to do something with that material (summarise, critique, reformat, translate).

If you paste your methods draft and ask for a critique, the model has your actual claims to work with. If you ask it to write one from scratch, it's generating from generic patterns with no grounding in your study. The transform mode tends to be more reliable, and we'll build on this distinction throughout the course.

## Try this: context continuation (5-8 min)

Take a paragraph you've written recently - an introduction, a methods section, an email to a collaborator. Anything where you know what comes next.

Delete the last sentence or two. Paste what remains into a chat LLM and ask: "Continue this text for one paragraph."

Compare the continuation to what you actually wrote. Notice:

- Did the model match your style? Where did it miss?
- Did it add new claims? If so, were they true?
- Did it flatten any nuance - simplify a point you'd made carefully?
- Would a reader notice the switch?

If you want to push this further, try it with two different models and compare their continuations to each other and to your original.

**Journal prompt**

Go back to your tool comparison from Monday. Now that you know more about how LLMs work - generating plausible continuations based on patterns, not looking things up - does anything about those results make more sense? Write a few lines connecting what you observed to what you've learned.
