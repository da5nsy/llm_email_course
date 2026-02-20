**Subject:** [GAIR] Prompt hacks are mostly theatre

---

Week 3 of 10 - Prompting, ideation, and the convergence trap

---

If you search for "prompting tips" you'll find thousands of results. Add "think step by step." Use the STAR framework. Tell the model it's an expert. Threaten it with job loss (really). The internet has turned prompting into a kind of folk magic - incantations that supposedly unlock hidden capabilities.

Most of this is theatre. Some of it used to matter more, with earlier, less capable models. But the core insight is simpler than the cottage industry suggests: the better you specify what you want, the more useful the output tends to be. That's not a secret hack. It's how communication works with any collaborator, human or otherwise.

**Clarity beats tricks**

The single most reliable way to get better AI output is to be clearer about what you're asking for. This sounds obvious, but in practice most prompts are vague. "Summarise this paper" could mean a one-sentence gist, a structured abstract, or a 500-word overview highlighting methodological choices. The model will guess what you meant, and it will guess confidently.

This is worth thinking about not because you need to master some "prompting framework" but because forcing yourself to specify what you actually want is useful in its own right. What do you need from this summary? Who is it for? What matters and what doesn't? The exercise of writing a clear prompt often clarifies your own thinking, which is half the value.

That said, there's a place for vague prompts too. Sometimes you don't know what you want yet, and a loose question like "what are the main debates around X?" can surface angles you hadn't considered. The trick is knowing which mode you're in: exploring or executing. Vague prompts are fine for exploration. For execution, specificity pays off.

**Roles, examples, and constraints**

A few prompting moves do reliably change outputs, and they're worth knowing about.

**Roles** (or personas): telling the model to respond "as a methodologist" or "as a skeptical reviewer" adjusts the style and focus of the output. The model doesn't become an expert. But it shifts which patterns get activated, which can produce noticeably different results. A "methods consultant" persona will focus on design choices; an "interested layperson" persona will skip the jargon.

**Few-shot examples**: showing the model what you want by including 1-3 examples of the desired output. This is particularly useful when you need a specific format or style that's hard to describe in words. If you want a particular kind of annotation, show it one. The model picks up on patterns fast.

**Constraints**: specifying what you don't want, or setting boundaries on the output. "No more than 200 words." "Use only information from the text I provided." "If you're not confident about something, say so." These don't always work perfectly, but they shift the distribution of outputs in your direction.

None of these are revolutionary. They're ways of being specific about what you need. The most sophisticated prompting technique in the world won't fix a request that isn't clear about its purpose.

**Thinking modes and model differences**

Many models now offer a "thinking" or "extended reasoning" mode (sometimes called chain-of-thought). When activated, the model works through a problem step by step before giving its final answer. This genuinely helps with certain tasks - anything involving logic, maths, multi-step reasoning, or planning. It doesn't guarantee correctness, and it adds latency and cost, but it can meaningfully improve output quality on hard problems.

For simpler tasks - summarising, reformatting, brainstorming - thinking mode usually adds little. It's a tool for when the task is genuinely difficult, not a "make everything better" button.

Meanwhile, different models still have genuinely different strengths. Some are better at creative generation, others at careful analysis. Some follow instructions more precisely, others take more initiative. Rather than searching for the one best model, it's worth thinking of them as an ensemble of specialists. If one model's output isn't working for a task, try another before concluding that AI can't help.

**Interaction over incantation**

Here's the real shift in thinking about prompting: the goal is conversation, not a perfect one-shot prompt. The most effective AI use I've seen in research involves back-and-forth - an initial prompt, then refinement. "This is close but too general - can you focus on the methodological criticisms?" or "Good list, but you missed [X] - what else is in that space?"

Multi-turn interaction lets you steer the output iteratively, which is both more effective and more forgiving than trying to get everything right in a single prompt. It also means that prompting "skill" matters less than domain knowledge. Knowing what good output looks like - and being able to recognise when you're not getting it - is more valuable than any formatting trick.

[ADD PERSONAL EXPERIENCE: a specific example of multi-turn refinement from your own work]

## Try this: iteration ladder (10-12 min)

Pick a real research task - something you actually need to do. A literature summary, a critique of a methods section, a draft of an email to a collaborator, a set of survey items. Anything where you'll be able to judge the quality of the output.

Run four prompts on the same task, in order:

1. **Vague:** Ask for what you want in the most casual, unspecific way. ("Summarise this paper." / "Help me write about X.")
2. **Constrained:** Add specifics. What format? What length? What should it focus on? What audience? ("Summarise this paper in 200 words, focusing on methodology and limitations, for a reader familiar with the field.")
3. **Role-based:** Add a persona. ("You are a methods consultant reviewing this paper for a grant panel. Summarise in 200 words, focusing on methodology and limitations.")
4. **Few-shot:** Include an example of what you want the output to look like. Paste in a summary you've written (or one you like) and ask for the same treatment of a different paper.

Compare the four outputs. Where did added specificity help most? Was there a point of diminishing returns? Did the few-shot example change the output more than the role, or the other way around?

You might find that the jump from vague to constrained is the biggest improvement, and that roles and examples add more subtle calibration. Or you might find that for your particular task, few-shot examples are transformative. The point is to develop your own sense of what moves the needle for your work, rather than following generic advice.

**Journal prompt**

Which prompting moves - if any - actually changed the quality of your results? Was there a prompt where added specificity made things worse (too constrained, too narrow)? What does this tell you about how you want to work with these tools?
