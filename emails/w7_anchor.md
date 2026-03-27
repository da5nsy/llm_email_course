**Subject:** [GAIR] The jagged frontier: spectacular and silently wrong

---

Week 7 of 10 - From browser to local: introducing agents

---

If you tried an agent this week, you probably had a moment where it did something impressively useful. Read your files, understood the structure, produced output that was specific to your project. Maybe it saved you hours of work in ten minutes. Maybe it identified something you'd missed.

You might also have had a moment where it got something wrong that seemed very simple to you. Where it failed to implement a statistical test you deemed easy to code. Where it went down a rabbit hole trying to fix PowerPoint formatting, spending 20 minutes on a formatting task that would have taken you 30 seconds.

This is the pattern worth paying attention to.

**The jagged frontier**

Ethan Mollick uses the phrase "jagged frontier" to describe AI capability: it's not uniformly good or uniformly bad. The boundary between what works and what doesn't is irregular and hard to predict in advance. A model that writes flawless analysis code might struggle with a simple formatting task. One that summarises 20 papers brilliantly might miss an obvious contradiction between two of them.

The practical implication is that you can't judge from first principles what an agent will handle well. You have to try it. Your frontier will be different from your colleague's, because it depends on your field, your tasks, your file types, and the specific tools you use. And it shifts constantly - the models you're working with now are the worst models you'll ever work with. What fails today may work in six months. Also, remember that LLMs are not deterministic; each run will be slightly different.

This means the right response isn't to write off agents based on one bad experience, or to trust them completely based on one good one. It's to keep experimenting, keep notes on what works and what doesn't, and expect to be surprised. It's also important to remember that there are many ways to achieve the same goal. Agents might be worse than you at PowerPoint, but better than you (and likely good enough) at creating polished code-based presentations, e.g. with *reveal.js*.

**Verification compounds with agents**

There's a separate challenge that comes with agents specifically. In a chat interface, you process each output individually - you read the paragraph, check the code, evaluate the suggestion. With agents, things move faster. The agent reads five files, makes three changes, runs the code, and presents you with results. By the time you're looking at the output, several steps have already happened that you didn't individually review.

This is why the generation-verification asymmetry from Week 2 matters even more here. Agents dramatically reduce generation costs. They can also help with verification - asking a second agent to check the first is a useful habit. But overall, verification costs are likely to increase, because there's more output to check and more steps where something could have gone quietly wrong.

**Mediocre work becomes trivially easy**

Agents make it easy to produce work that clears a basic quality bar. A literature summary that covers the right sources. Analysis code that runs without errors. A methods section that describes the right design. Getting from zero to "adequate" used to take time. Now it takes minutes.

But adequate isn't the standard in research. The difference between a competent literature review and one that identifies a genuine gap, between code that runs and code that answers the right question, between a methods section that's accurate and one that anticipates reviewer concerns - that difference still requires expertise. The top 10% of quality still needs you.

This shifts what your time is worth. If the agent handles the first draft in five minutes, your value isn't in producing that draft. It's in knowing what's wrong with it, what's missing, and what needs to change. That's a different skill from writing things from scratch, and for some tasks it might actually be harder. If you are driven by curiosity, like me, agents might also increase the number of exciting but unfinished projects you have around that are all lacking the final 10%.

**Verification strategies**

A few practical habits that help:

- **Spot-check specifics.** Don't just skim agent output for general plausibility. Pick specific claims or numbers and verify them against your source material. If the agent says "7 of 12 participants reported X," check whether it's really 7 of 12.
- **Ask the agent to flag its own uncertainties and to double-check.** Many agents will tell you where they're less confident if you ask. "Which parts of this output are you least sure about?" won't catch everything, but it's a useful first filter. Similarly, asking another agent (or a new instance of the same agent) to double-check outputs can highlight issues.
- **Make reports reproducible:** Many of us have heard of tools to write reproducible papers, where numbers are not copy-pasted but filled in by in-line code. This used to be rather fiddly and hasn't caught on widely - but with agents, it is easier and makes it less likely that you rely on outdated figures, or that the agent messes up when copying between data analysis and the manuscript.
- **Run sanity checks on the whole, not just the parts.** Does the overall picture make sense given what you know? Sometimes individual elements are correct but the synthesis is misleading.
- **Compare against your own understanding.** Before reading the agent's output in detail, write down what you'd expect to find. Then compare. Discrepancies are where the interesting checks are.

None of these are foolproof. Domain knowledge remains the best verification tool, which creates an uncomfortable implication: agents are most useful to people who could have done the work themselves (even if it would have taken longer). If you couldn't evaluate the output, the speed doesn't help you - it just means you get to wrong answers faster.

**Qualitative data analysis: a sidebar**

If you work with qualitative data, you may be wondering how agents fit. The short answer: agents can help with some phases of qualitative analysis, but the fit depends heavily on your epistemological commitments.

For keyword detection, surface-level categorisation, and organising large volumes of text, agents perform very well. For interpretive or latent coding - the kind where a code emerges from repeated engagement with the data rather than from a predefined list - they're weaker. They tend to generate more literal, descriptive codes than a (good) human researcher would, and they can miss the kind of meaning that only becomes visible through sustained immersion in the context. At least for now.

For reflexive qualitative approaches specifically, there are unresolved tensions. If the method requires you to bring your own perspective and positionality to the analysis, outsourcing interpretation to an AI raises fundamental questions about what the analysis actually is. These debates are active and ongoing. If you're interested, [Ibrahim and Voyer (2026)](https://doi.org/10.1177/14687941251390794) provide a useful starting point.

For now, it might be most interesting (and defensible) to use LLMs as a secondary check: run your own coding first, then see what the AI flags that you might have missed.

## Try this: evaluate agent output (5-8 min)

Take the output from Monday's exercise - or any output you've generated with an agent or extended AI session.

1. Identify two things the agent got right that saved you real time. Be specific: what would you have had to do manually?
2. Identify one thing it got wrong or oversimplified. How did you spot it?
3. Ask yourself: if you weren't already familiar with this material, would you have caught the error?
4. Identify one thing you cannot yet honestly assess in full. Does it matter enough to spend the time to dig into? How do you decide?

If you didn't try Monday's exercise, you can use any AI-generated output from the course so far. The question is the same: where was the AI reliably helpful, and where did it need your expertise to catch a problem?

**Journal prompt**

How would you explain to a colleague what the agent did and what you did? Where's the line between "the AI helped" and "the AI did the work"? (How) is that different from collaborative work with another researcher?
