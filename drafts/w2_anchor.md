**Subject:** [GAIR] Why it tells you what you want to hear

---

Week 2 of 10 - Confident errors: hallucination, sycophancy, epistemic vigilance

---

If the hallucination hunt on Monday made you less trusting of AI-generated facts, good. But fabrication isn't the only way these tools mislead you. There's a subtler one: agreement.

Ask an AI what it thinks of your research idea, and it will almost certainly tell you it's promising. Describe a study design and ask for feedback, and most of the response will be encouraging. This isn't because your ideas are uniformly brilliant (sorry). It's because, as we discussed last week, models are trained to produce responses that humans rate highly - and humans tend to rate agreeable, supportive responses more highly than critical ones.

This tendency has a name: **sycophancy**. The most extreme versions have been reined in (early ChatGPT versions would enthusiastically endorse almost anything), but the default tilt toward agreement is still there. It shows up as praise where critique would be more useful, and as a tendency to echo whatever framing you provide rather than questioning it.

**Why this matters for research**

In everyday use - drafting emails, brainstorming - sycophancy is a mild annoyance. In research, it's a real problem. If you use AI to stress-test an argument and it mostly tells you the argument is strong, you might mistake that for validation. You haven't received a critical review; you've received a mirror.

This gets worse the more you interact. Remember from last week that models respond to the full conversation, not just your last message. Over a long exchange, your framing accumulates in the context window. The model starts to sound more like you - reinforcing your assumptions rather than challenging them. Sycophancy and context drift work together.

**What shapes the outputs you get**

Beyond the RLHF training that pushes models toward agreement, there's another source of bias worth knowing about: training data. Models learn from what's in their training corpus, which means they reflect the patterns, gaps, and biases of that data. Topics that are well-covered in English-language internet text get better responses. Niche subfields, recent publications, and work in other languages are underrepresented. Models also have knowledge cut-offs - they don't know about events or publications after their training data ends, though this boundary is increasingly blurred as models are connected to web search.

None of this means AI output is useless. It means the errors are systematic, not random. Knowing the shape of the bias helps you compensate.

**A practical rule: the generation-verification asymmetry**

Here's a framework that helps decide when AI assistance is worth the risk.

AI is most useful when generation is costly for you but verification is cheap. Writing a first draft of boilerplate text, producing code for a standard analysis, generating a list of potential search terms - these are tasks where the AI's output might be imperfect, but you can check it quickly. The time saved in generation outweighs the cost of verification.

AI is riskiest when verification is hard or expensive. If you can't easily tell whether the output is correct - because it's outside your expertise, because checking requires significant effort, or because errors would be costly - then the confident tone becomes a liability rather than a convenience.

This asymmetry should shape which tasks you hand to AI and how much checking you invest. We'll return to it throughout the course.

## Try this: sycophancy demo + high-ROI audit (8-10 min)

**Part 1: See it for yourself (2 min)**

Take one of your research ideas - a hypothesis, a study design, even a half-formed question. Prompt an AI with: "Praise this idea. Assume it's correct and explain why it's promising." Read the response. Then try: "Now attack this idea. Assume it's flawed and explain why it would fail."

Compare the two. Notice how completely the model switches stance. Neither response is "what the AI thinks." Both are plausible continuations of the prompt you gave.

**Part 2: Where does AI help you most? (5-8 min)**

List 5 research tasks you do regularly. For each one, rate:

- How long does it take you to do this from scratch?
- If an AI did it, how easy would it be to check the result?
- How bad would it be if the result were wrong and you didn't catch it?

Identify 2 tasks where AI is high-ROI (costly to generate, cheap to verify) and 1 where it's a danger zone (hard to verify, costly if wrong). Keep this list - it's the beginning of the personal SOP we'll build toward in Week 10.

**Further reading**

- [Why language models hallucinate](https://openai.com/index/why-language-models-hallucinate/) - OpenAI's own explanation of the problem.

**Journal prompt**

Which of your regular tasks have cheap verification? Where is verification expensive? Has the sycophancy demo changed how you read AI responses?
