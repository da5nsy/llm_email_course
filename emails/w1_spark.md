**Subject:** [GAIR] Your AI baseline

---

Week 1 of 10 - What LLMs are (and aren't)

---

You already use AI for something. Maybe you've asked ChatGPT to explain a statistical method, or had Claude draft an email you didn't want to write, or quietly pasted a paragraph into Gemini to see if it could say it better. Maybe you've done more than that, and started experimenting with AI agents. Maybe you've done less and feel behind.

Whatever your starting point, you have a sense - however rough - of what AI is good for and where it falls apart. That sense is worth examining before this course adds new information on top of it.

There's a real reason AI has spread so fast through research workflows. It can summarise a dense paper in seconds, suggest analysis approaches you hadn't considered, help you wrestle a rough draft into shape, or produce working code for a task that would have taken you an afternoon to look up. These aren't small things. When AI works, it saves time and mental effort.

But it also gets things wrong - sometimes obviously, sometimes not. And that's the tension this course is built around: AI tools are productive enough that ignoring them has a cost, but unreliable enough that trusting them uncritically has a bigger one. As AI tools become better, the precise pattern is shifting continuously, so that we can trust AI in some areas where it failed abysmally recently ... but the human touch will continue to matter (I hope).

This course does not come with a promise to automate your research. Similarly, I'm not going to tell you what AI can't do, given that such claims tend to age poorly. Instead, I am hoping that the next ten weeks offer a chance to reflect, experiment, and develop habits that allow you to work effectively with a range of AI tools - in a way that matches your values, your style, and your field of research. But first, let's start with some groundwork.

**What LLMs actually do**

Large language models (LLMs) generate text that would be a plausible continuation of whatever you give them. More technically, they engage in next-token-prediction. That's it (mostly). Fortunately, they don't work like early text completion suggestions on smartphones by just looking at the last 2-3 words; instead they can consider hundreds of thousands of words when they decide what comes next. Nevertheless, when you ask ChatGPT a question, it doesn't look up an answer in a database. It produces text that looks like a good answer would look, based on patterns learned from enormous amounts of text during training. Often that text is useful. Sometimes it's wrong in ways that are hard to spot, because the wrongness is wrapped in confident, well-structured prose.

The confidence you hear in an AI response - the authoritative tone, the clear structure, the lack of hedging - is a style feature, not a reliability signal. A model can be completely wrong and sound exactly as confident as when it's right.

In early days, this led to hilarious outputs - like the first time I used ChatGPT for data analysis, and asked it to create a correlation table. It struggled to read the data file, so just decided to guess and then hard-code the correlations into the code, which produced a convincing table. Those days have mostly gone, but references are still frequently garbled. There are just many plausible ways to continue once you start writing down a page number.

You might wonder how next-word prediction can actually be useful. It can sound trivial, but you'll likely be surprised by how much you can capture just by learning which words go together (I still am). Basic LLMs can do a lot with this - but they can also get things confidently wrong when the probabilities don't align. There are ways to make this more reliable - reasoning modes, grounding in your own documents, agentic AI where models validate their output. We'll get to all of that later in the course.

**Different tools, different behaviour**

Each LLM is trained on different data, optimised for different types of answers, and following different system instructions that guide *how* it will approach answers. These can feel like distinct personalities when it comes to how flattering or critical models are - and at any one time, some models will be better at certain tasks than others. While it is not necessary to try to stay current on all models, unless you are working on a specific frontier, it is worth playing around with different models from time to time. Also, remember that so far, many claims about "AI can't do X" have turned into "AI couldn't do X yet" - so if something matters to your work but didn't work last time you tried, it's still worth retrying after some time.

## Try this: AI autobiography + tool comparison (10-15 min)

This is a two-part exercise. One is looking reflective, the other hands-on.

**Part 1: AI autobiography**

Write six bullet points - quick and honest, no need to polish:

- What do you currently use AI for in your research or work?
- What benefits have you noticed?
- What's gone wrong? (A bad output, a wasted afternoon, a moment of doubt)
- What's your biggest worry about AI in research?
- What are your current red lines - tasks you refuse to hand to AI?
- What do you want to get out of this course?

Save these somewhere you can find them again. We'll come back to them in Week 10, and the contrast is often surprising. (If you want to, you can paste these questions into an LLM and let it interview you, maybe even in voice mode. That might be more engaging than typing out answers.)

**Part 2: Tool comparison**

Pick a topic you know well - well enough to spot errors - and ask two or three different AI tools the same question. Choose one of these prompts (or adapt to your field):

- "Explain [your topic] in plain language for a smart non-expert."
- "Recommend 6 foundational readings for [your topic] and explain why each matters."
- "Propose 3 plausible hypotheses about [your topic] and how you'd test them."

If you're not sure what to ask about, try something specific to your methods: "What are the main criticisms of [a method you use regularly]?" You'll likely know enough to judge the answer. If you are using LLMs regularly, maybe use this opportunity to try out some models you haven't worked with yet. Most will offer a free tier that is more than sufficient for this.

As you read the responses, note:

- What was genuinely helpful?
- What was wrong? (Check specifics - names, dates, claims, citations)
- What sounded convincing but, on reflection, was vague or unsupported?
- Where did the tools differ from each other?

Don't worry about being systematic. Even a rough comparison will give you a feel for how these tools differ and where your expertise lets you see through the surface.

**A practical note on tools:** I don't recommend specific models in this course - the landscape shifts too fast. The main commercial providers are OpenAI (**ChatGPT**), Google (**Gemini**), and Anthropic (**Claude**). On the open-source side, **DeepSeek**, **Kimi**, **GLM**, **Minimax** and **Qwen** are strong options, with **Mistral** and Meta's **Llama** also worth knowing about. Leaderboards like [Artificial Analysis](https://artificialanalysis.ai/leaderboards/models) can help you compare, and multi-model platforms like [t3.chat](https://t3.chat/) let you try several without multiple subscriptions. Most exercises in this course work with free tiers, though you may need to switch between providers to stay within usage limits ... and if you run into something "AI can't do" it's worth double-checking that conclusion with the best models.

**Want to share your thoughts and connect with others?**

We have created a channel on the FORRT Slack specifically for this course. Join it [here](ADD LINK) and say hello.

**Start your journal**

Throughout this course, we'll ask you to jot down observations and reflections. Nothing formal - a Google Doc, a notebook, whatever works. Copy your AI autobiography in as your first entry. We'll come back to it.
