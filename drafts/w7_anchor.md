**Subject:** [GAIR] The jagged frontier: spectacular and silently wrong

---

Week 7 of 10 - From browser to local: introducing agents

---

If you tried an agent this week, you probably had a moment where it did something impressively useful. Read your files, understood the structure, produced output that was specific to your project. Maybe it saved you an hour of work in ten minutes. Maybe it identified something you'd missed.

You might also have had a moment where it got something wrong. Not dramatically wrong - that's easy to catch. Subtly wrong. A summary that sounds right but misses the key distinction. A table that's well-structured but conflates two different measures. Code that runs cleanly but handles missing data in a way that changes your sample without telling you.

This is the pattern worth paying attention to.

**The jagged frontier**

Ethan Mollick uses the phrase "jagged frontier" to describe something important about AI capability: it's not uniformly good or uniformly bad. It's spectacular at some tasks and silently wrong at others, and the boundary between the two is irregular and hard to predict.

Agents make this more consequential. In a chat interface, you process each output individually. You read the paragraph, you check the code, you evaluate the suggestion. With agents, things move faster. The agent reads five files, makes three changes, runs the code, and presents you with results. By the time you're looking at the output, several steps have already happened that you didn't individually review. The stakes for each individual step are lower - but the compound risk of not checking is higher.

This is why the generation-verification asymmetry from Week 2 matters even more here. Remember the principle: AI is most useful where generation is costly for you and verification is cheap. Agents dramatically reduce generation costs. They don't change verification costs at all. If anything, they increase them, because there's more output to check.

**Mediocre work becomes trivially easy**

Agents make it easy to produce work that clears a basic quality bar. A literature summary that covers the right sources. Analysis code that runs without errors. A methods section that describes the right design. Getting from zero to "adequate" used to take time. Now it takes minutes.

But adequate isn't the standard in research. The difference between a competent literature review and one that identifies a genuine gap, between code that runs and code that answers the right question, between a methods section that's accurate and one that anticipates reviewer concerns - that difference still requires expertise. The top 10% of quality still needs you.

This shifts what your time is worth. If the agent handles the first draft in five minutes, your value isn't in producing that draft. It's in knowing what's wrong with it, what's missing, and what needs to change. That's a different skill from writing things from scratch, and for some tasks it might actually be harder.

**Verification strategies**

A few practical habits that help:

- **Spot-check specifics.** Don't just skim agent output for general plausibility. Pick specific claims or numbers and verify them against your source material. If the agent says "7 of 12 participants reported X," check whether it's really 7 of 12.
- **Ask the agent to flag its own uncertainties.** Many agents will tell you where they're less confident if you ask. "Which parts of this output are you least sure about?" won't catch everything, but it's a useful first filter.
- **Run sanity checks on the whole, not just the parts.** Does the overall picture make sense given what you know? Sometimes individual elements are correct but the synthesis is misleading.
- **Compare against your own understanding.** Before reading the agent's output in detail, write down what you'd expect to find. Then compare. Discrepancies are where the interesting checks are.

None of these are foolproof. Domain knowledge remains the best verification tool, which creates an uncomfortable implication: agents are most useful to people who could have done the work themselves (even if it would have taken longer). If you couldn't evaluate the output, the speed doesn't help you - it just means you get to wrong answers faster.

**Qualitative data analysis: a sidebar**

If you work with qualitative data, you may be wondering how agents fit. The short answer: agents can help with some phases of qualitative analysis, but the fit depends heavily on your epistemological commitments.

For keyword detection, surface-level categorisation, and organising large volumes of text, agents perform reasonably well. For interpretive or latent coding - the kind where a code emerges from repeated engagement with the data rather than from a predefined list - they're much weaker. They tend to generate more literal, descriptive codes than a human researcher would, and they can miss the kind of meaning that only becomes visible through sustained immersion.

For reflexive qualitative approaches specifically, there are unresolved tensions. If the method requires you to bring your own perspective and positionality to the analysis, outsourcing interpretation to an AI raises fundamental questions about what the analysis actually is. These debates are active and ongoing. If you're interested, Morgan (2023) is a useful starting point on AI as assistant in early phases of interpretive work. [NEEDS CHECK: Morgan 2023 reference details]

The most defensible current use is probably as a secondary check: run your own coding first, then see what the AI flags that you might have missed. Not as a primary coder.

## Try this: evaluate agent output (5-8 min)

Take the output from Monday's exercise - or any output you've generated with an agent or extended AI session.

1. Identify two things the agent got right that saved you real time. Be specific: what would you have had to do manually?
2. Identify one thing it got wrong or oversimplified. How did you spot it?
3. Ask yourself: if you weren't already familiar with this material, would you have caught the error?

If you didn't try Monday's exercise, you can use any AI-generated output from the course so far. The question is the same: where was the AI reliably helpful, and where did it need your expertise to catch a problem?

**Journal prompt**

How would you explain to a colleague what the agent did and what you did? Where's the line between "the AI helped" and "the AI did the work"?
