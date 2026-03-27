**Subject:** [GAIR] The grunt work was training: what agents can't replace

---

Week 8 of 10 - Agents for research workflows

---

By now, you've seen what agents can do. They read your files, write your code, extract information from your documents, iterate when things go wrong. With a good specification, they produce output that's genuinely useful. It's natural to look at this and think: if the agent can do the execution, what's left for me?

Quite a lot, it turns out. But not always the parts you'd expect.

**The grunt work was training**

Kiran Garimella made this point sharply in [a recent essay](https://kirangarimella.substack.com/p/ai-agents-and-academia): the tasks we used to call "grunt work" in research - cleaning datasets, writing basic analysis code, formatting tables, chasing down references - were also how we built competence. You learn what messy data looks like by cleaning it. You understand statistical models by implementing them badly and fixing the errors. You develop judgment about sources by reading a lot of mediocre ones.

When agents do these tasks in minutes, that's more efficient. But the learning that used to come bundled with the work doesn't transfer automatically. A researcher who has never cleaned a dataset may not recognise when an agent has cleaned it wrong. Someone who has never written analysis code from scratch may not know which questions to ask about the code an agent produces.

This isn't a reason to refuse to use agents. It's a reason to be thoughtful about what you're giving up when you delegate, especially early in your career or when entering an unfamiliar domain. The efficiency gain is real. The skill gap it might create is also real. How (and if) critical engagement with AI outputs is possible in areas where we don't understand the production process is a fundamental question for education - but for now, one we will all need to explore critically as we go along.

**What stays human**

If execution becomes cheap, what becomes more valuable?

*The questions you ask.* Agents are good at answering well-specified questions. They're not (yet) good at knowing which questions matter. Identifying a gap in the literature, noticing a pattern that doesn't fit the prevailing theory, designing a study that tests something nobody thought to test - these are still human strengths, and they depend on the kind of deep familiarity that comes from sustained engagement with a field. AI can obviously scan "limitations and future directions" sections of recent papers and build ideas from there, but these still need to be ranked tastefully.

*The data you can uniquely access.* Agents can analyse any dataset you give them, but they can't build the relationships that get you access to restricted data, run the experiment, or conduct the interviews. The value of data you collected yourself - or that only you have permission to use - increases when analysis becomes cheap. Conversely, creative ideas for combining publicly accessible datasets, or for extracting datasets from unstructured messy data, become more feasible, and thus more valuable.

*Domain judgment.* When the agent produces a result, you need to know whether it makes sense. Not just statistically, but substantively. Does this effect size seem reasonable? Is this interpretation consistent with what we know from adjacent literatures? Would this finding replicate? That judgment comes from years of reading, thinking, and arguing with colleagues. An agent can share one perspective on that, but ultimately you need to make the call.

*Ethical reasoning.* Agents don't have stakes in the outcome. They don't feel the weight of publishing a finding that might influence policy, or the responsibility of handling data from vulnerable populations. The ethical dimensions of research require a kind of judgment that isn't about getting the right answer - it's about caring what happens next. Not in the sense of (only) pursuing specific results, but in terms of how to communicate them responsibly.

*Orchestration.* Designing a research programme, choosing which questions to pursue, coordinating people and tools toward a coherent goal. Frontier agents can already work for weeks on a hard problem (at vast cost, for now), but deciding what problems matter and how they fit together is still yours.

**Agent supervision as a skill**

Here's something that might sound odd: working well with agents is itself a skill, and it's different from the skills it's replacing.

When you write code yourself, you think about the problem step by step. When you supervise an agent writing code, you need to think about the specification, evaluate the output, and catch errors in someone else's reasoning. That's more like supervising a research assistant than doing the work yourself. It requires a different kind of attention.

Some people find this easier. Others find it harder. It's common to feel less engaged when reviewing output than when producing it - and that disengagement is precisely when errors slip through. Building the discipline to stay critical when the work feels "done" is part of learning to use agents well. Building the clarity of thought and communication it takes to instruct an agent stands us in good stead when leading human collaborators as well.

**Your jagged frontier is personal**

What you can safely delegate to an agent depends on what you already know. An experienced statistician can delegate code-writing to an agent and verify the output efficiently, because they know what the code should do. A researcher who's never run that analysis can't verify it the same way.

This means your "jagged frontier" - the boundary between tasks you can safely delegate and tasks you shouldn't - is specific to you. It depends on your expertise, your domain, and the particular task. And it moves over time: as you learn more, you can delegate more safely. As tools improve, the frontier shifts again.

The honest answer to "should I let the agent do this?" is usually: can you evaluate whether it did it right? (And maybe more personally: is this work you actually want to give away?) If yes, delegate and verify. If not, either learn enough to evaluate it, or do it yourself. Remember, though, that verification doesn't always require generation competence. Agents can build interactive visualisations, web apps, and other small software tools that are easy to validate by using them, even if you couldn't have built them yourself.

## Try this: map your frontier (5-8 min)

1. List 10 research tasks you do regularly. Consider mundane tasks (formatting, file management) with substantive ones (analysis decisions, interpretation, writing arguments).
2. For each, classify it: **human-only** (you wouldn't trust an agent with this) / **AI-supported** (useful, but needs iteration) / **AI-outsourced** (agent can handle it reliably, you just review).
3. For each AI-supported task, write one cheap verification check you'd run on the output.
4. Circle any task where you'd lose important learning by outsourcing it. Be honest. The efficiency gain might still be worth it - but name what you're trading away.

Look at your list. How does it compare to the high-ROI audit from Week 2? Has your sense of what's delegable changed?

**Journal prompt**

Which tasks are you tempted to outsource but probably shouldn't? Why? What would you need to learn before you could safely delegate them?
