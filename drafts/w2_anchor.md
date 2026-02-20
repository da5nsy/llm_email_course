**Subject:** [GAIR] Why it tells you what you want to hear

---

Week 2 of 10 - Confident errors: hallucination, sycophancy, and the need to stay vigilant

---

If the hallucination hunt on Monday made you less trusting of AI-generated facts, good (unless you've come to believe that only entirely accurate tools are useful). But fabrication isn't the only way these tools mislead you. There's a subtler one: agreement.

Ask an AI what it thinks of your research idea, and it will almost certainly tell you it's promising. Describe a study design and ask for feedback, and most of the response will be encouraging. This isn't because your ideas are uniformly brilliant (sorry). It's because, as we discussed last week, models are trained to produce responses that humans rate highly - and humans tend to rate agreeable, supportive responses more highly than critical ones.

This tendency has a name: **sycophancy**. The most extreme versions have been reined in (early ChatGPT versions would enthusiastically endorse almost anything), but the default tilt toward agreement is still there in most models. It shows up as praise where critique would be more useful, and as a tendency to echo whatever framing you provide rather than questioning it.

**Why this matters for research**

In everyday use - drafting emails, brainstorming - sycophancy is a mild annoyance. In research, it's a real problem. If you use AI to stress-test an argument and it mostly tells you the argument is strong, you might mistake that for validation. You haven't received a critical review; you've looked into a distorting mirror.

This gets worse the more you interact. Remember from last week that models respond to the full conversation, not just your last message. Over a long exchange, your framing accumulates in the context window. The model starts to sound more like you - reinforcing your assumptions rather than challenging them. Sycophancy and context drift work together.

**What shapes the outputs you get**

Beyond the human-feedback training that pushes models toward agreement, there's another source of bias worth knowing about: training data. Models learn from what's in their training corpus, which means they reflect the patterns, gaps, and biases of that data. Topics that are well-covered in English-language internet text get better responses. Niche subfields, recent publications, and work in other languages are underrepresented. Models also have knowledge cut-offs - they don't know about events or publications after their training data ends, though this boundary is increasingly blurred as models are connected to web search.

So if AI output may be hallucinated, sycophantic and biased, where does that leave us? In my practical experience, still with something that is often very useful. It's also worth remembering that different models have different default personalities here - some are more willing to say "I'm not sure" or push back on your framing, while others default to confident agreement regardless. If you find one model particularly sycophantic or hallucination-prone, try another, at least for the task at hand.

There's a fancy term for this calibrated scepticism - *epistemic vigilance* - and an even older one: the Royal Society's motto *nullius in verba*, take nobody's word for it. The practice is simpler than the labels: check before you trust, and know when checking matters most.

**A practical rule: the generation-verification asymmetry**

LLMs are great at generating (or modifying) text. Verification remains our task. That asymmetry helps me decide when to use them.

LLMs are most useful when generation is costly for you but verification is cheap. Writing a first draft of boilerplate text, producing code for a standard analysis, generating a list of potential search terms - these are tasks where the AI's output might be imperfect, but you can check it quickly. The time saved in generation outweighs the cost of verification.

AI is riskiest when verification is hard or expensive. If you can't easily tell whether the output is correct - because it's outside your expertise or because checking requires significant effort - and if errors would be costly, then the confident tone becomes a liability rather than a convenience.

This asymmetry also shapes why different people have different levels of success with AI. If you know how to write well, it is easier to verify AI output and thus to benefit from generation. If you know how to review and test code effectively, AI generated code becomes more valuable. In that sense, we are not being replaced (yet).

## Try this: sycophancy demo + high-ROI audit (8-10 min)

**Part 1: See it for yourself (2 min)**

Take one of your research ideas - a hypothesis, a study design, even a half-formed question. Prompt an AI with: "Praise this idea. Assume it's correct and explain why it's promising." Read the response. Then (in a new chat) try: "Now attack this idea. Assume it's flawed and explain why it would fail." Finally (in a new chat), ask "Do you think this is a good idea?"

Compare the three. Notice how completely the model switches stance. None of the responses are "what the AI thinks." All are plausible continuations of the prompt you gave. Maybe all of them included some worthwhile nuggets?

**Part 2: Where does AI help you most? (5-8 min)**

List 5 research tasks you do regularly. For each one, rate:

- How long does it take you to do this from scratch?
- If an AI did it, how easy would it be to check the result?
- How bad would it be if the result were wrong and you didn't catch it?

Identify 2 tasks where AI is high-ROI (costly to generate, cheap to verify) and 1 where it's a danger zone (hard to verify, costly if wrong). Keep this list - it's the beginning of the personal "operating procedure" we'll build toward in Week 10.

**Further reading**

- [Why language models hallucinate](https://openai.com/index/why-language-models-hallucinate/) - OpenAI's own explanation of the problem.

**Journal prompt**

Which of your regular tasks have cheap verification? Where is verification expensive? Has the sycophancy demo changed how you read AI responses? Make sure to also note your responses to Part 2 above so that you can return to them.
