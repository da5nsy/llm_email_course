**Subject:** [GAIR] What do you trust AI for (and why)?

---

Week 1 of 10 - What LLMs are (and aren't)

---

You already use AI for something. Maybe you've asked ChatGPT to explain a statistical method, or had Claude draft an email you didn't want to write, or quietly pasted a paragraph into Gemini to see if it could say it better. Maybe you've done more than that. Maybe you've done less and feel behind.

Whatever your starting point, you have a sense - however rough - of what AI is good for and where it falls apart. That sense is worth examining before this course adds new information on top of it.

There's a real reason AI has spread so fast through research workflows. It can summarise a dense paper in seconds, suggest analysis approaches you hadn't considered, help you wrestle a rough draft into shape, or produce working code for a task that would have taken you an afternoon to look up. These aren't small things. When AI works, it genuinely saves time and mental effort.

But it also gets things wrong - sometimes obviously, sometimes not. And that's the tension this course is built around: AI tools are productive enough that ignoring them has a cost, but unreliable enough that trusting them uncritically has a bigger one.

The most common mistake with generative AI isn't using it too much or too little. It's using it without noticing the pattern of when it helps and when it doesn't. Over the next ten weeks, we'll build that noticing into a habit. But first, a baseline.

**What LLMs actually do**

Large language models generate text that would be a plausible continuation of whatever you give them. That's it. That's the core operation. When you ask ChatGPT a question, it doesn't look up an answer in a database. It produces text that looks like a good answer would look, based on patterns learned from enormous amounts of text during training. Often that text is genuinely useful. Sometimes it's wrong in ways that are hard to spot, because the wrongness is wrapped in confident, well-structured prose.

The confidence you hear in an AI response - the authoritative tone, the clear structure, the lack of hedging - is a style feature, not a reliability signal. A model can be completely wrong and sound exactly as confident as when it's right.

[TODO: Add personal experience here - a time when AI confidence tripped you up, or a colleague's experience. E.g., a plausible-sounding citation that turned out to be fabricated, a statistic that was invented but felt right.]

**Different tools, different behaviour**

If you've only used one AI tool, you might think of "AI" as a single thing with a single personality. It's not. ChatGPT, Claude, Gemini, DeepSeek, and others are built by different companies, trained on different data, and optimised for different things. They have different strengths, different blind spots, and different failure modes.

[TODO: Add brief current comparison. Something like "Claude tends to be more cautious about uncertain claims; ChatGPT is often more willing to speculate; Gemini integrates web search more aggressively." Verify against current model behaviour at time of sending - this shifts fast.]

Treating each tool as a distinct collaborator rather than interchangeable instances of "AI" is one of the most practical things you can do early on. You wouldn't ask the same colleague for help with statistics and with qualitative coding without adjusting your expectations. Same principle.

## Try this: AI autobiography + tool comparison (10-15 min)

This is a two-part exercise. The first part is just for you; the second will give you something concrete to refer back to throughout the course.

**Part 1: AI autobiography**

Write six bullet points - quick and honest, no need to polish:

- What do you currently use AI for in your research or work?
- What benefits have you noticed?
- What's gone wrong? (A bad output, a wasted afternoon, a moment of doubt)
- What's your biggest worry about AI in research?
- What are your current red lines - tasks you refuse to hand to AI?
- What do you want to get out of this course?

Save these somewhere you can find them again. We'll come back to them in Week 10, and the contrast is often surprising.

**Part 2: Tool comparison**

Pick a topic you know well - well enough to spot errors - and ask two or three different AI tools the same question. Choose one of these prompts (or adapt to your field):

- "Explain [your topic] in plain language for a smart non-expert."
- "Recommend 6 foundational readings for [your topic] and explain why each matters."
- "Propose 3 plausible hypotheses about [your topic] and how you'd test them."

If you're not sure what to ask about, try something specific to your methods: "What are the main criticisms of [a method you use regularly]?" You'll know enough to judge the answer.

As you read the responses, note:

- What was genuinely helpful?
- What was wrong? (Check specifics - names, dates, claims, citations)
- What sounded convincing but, on reflection, was vague or unsupported?
- Where did the tools differ from each other?

Don't worry about being systematic. Even a rough comparison will give you a feel for how these tools differ and where your expertise lets you see through the surface.

**A practical note on tools:** We don't recommend specific models in this course - the landscape shifts too fast. The main commercial providers are OpenAI (**ChatGPT**), Google (**Gemini**), and Anthropic (**Claude**). On the open-source side, **DeepSeek**, **Kimi**, **GLM**, and **Qwen** are strong options, with **Mistral** and Meta's **Llama** also worth knowing about. [TODO: Update to current leading open-source models at time of sending.] Leaderboards like [Artificial Analysis](https://artificialanalysis.ai/leaderboards/models) can help you compare, and multi-model platforms like [t3.chat](https://t3.chat/) let you try several without multiple subscriptions. Most exercises in this course work with free tiers, though you may need to switch between providers to stay within usage limits. [TODO: Check whether free vs paid tier difference is still significant enough to mention at time of sending.]

[TODO: Add FORRT Slack invitation - share your AI autobiography or one surprising finding from the comparison.]

**Journal prompt**

What do you currently trust AI for? What are your red lines? Write a few sentences - you'll want to compare these with your answers at the end of the course.
