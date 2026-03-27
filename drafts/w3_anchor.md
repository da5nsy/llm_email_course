**Subject:** [GAIR] Better ideas, more of the same

---

Week 3 of 10 - Prompting, ideation, and the convergence trap

---

Based on the exercised so far, you should be able to specify what you want, assign roles, provide examples. Your AI outputs might be more relevant and more focused than they were two weeks ago.

That's good. But here's a different kind of question: what if the problem isn't that AI gives bad ideas, but that it gives everyone the same ones?

**AI as sparring partner**

One of the most appealing uses of AI in research is as a thinking partner. Bouncing ideas, generating alternatives, stress-testing arguments. And it can be good at this - particularly at making connections across fields, suggesting angles you hadn't considered, and producing a first pass at critique that gives you something to react to.

But there's a structural issue underneath the usefulness.

**The convergence problem**

[A 2025 study](https://doi.org/10.1038/s41562-025-02173-x) found that when people used AI for creative tasks, the average quality of ideas went up - but the diversity went down. People working with AI produced more similar ideas than people working alone. Individual outputs got better; collective variety got worse (at least when the tasks didn't truly matter and they were working independently).

More concerningly, [a 2026 study](https://doi.org/10.1038/s41586-025-09922-y), analysing 41 million papers, found that AI-assisted research tends to cluster around popular topics and covers less intellectual territory than conventional research. The tools draw from the same training data, are optimised for the same notion of "helpful," and tend to nudge everyone toward the centre of the distribution, and toward areas already covered well in the training data.

This matters for research in a way it might not for marketing copy. If AI makes it easy for every researcher to produce competent-sounding ideas on trending topics, but harder to produce weird, unexpected, field-shifting work, that's a problem that won't show up at the individual level. Each person thinks their AI-assisted output is pretty good. The loss only becomes visible when you look across the field.

**Working against the grain**

The fix isn't to stop using AI for ideation. It's to use it deliberately, pushing against the tendency toward agreement and consensus.

**Socratic prompting** means asking the AI to challenge your thinking rather than confirm it. Instead of "What do you think of this hypothesis?", try "What are the strongest arguments against this hypothesis?" or "What would a critic from [rival theoretical tradition] say about this?" The model will still be drawing on mainstream patterns, but you're at least pointing it in a less comfortable direction.

**Adversarial prompting** goes further: ask for counter-hypotheses that explain the same pattern, confounding variables you might have missed, or boundary conditions where your argument falls apart. The model may not produce novel objections, but it can surface critiques that are easy to overlook when you're deep in your own framing.

**Pushing for unlikely ideas** tackles convergence more directly. LLMs default to one of the most probable responses, which is almost by definition the least original one. You can counter this by asking for quantity: "Give me 20 possible explanations for this pattern" forces the model past its first-instinct answers and into less obvious territory (and at this stage, verification is cheaper than generation, so that you can narrow down quickly). You can also be explicit: "What are some unlikely or unconventional explanations that most researchers wouldn't consider?" Another option is to run the same prompt through two or three different models - they draw on different training data and optimisation choices, so the overlap between their responses is often where the conventional wisdom lives, and the differences are where something interesting might be hiding.

None of these is a substitute for an actual colleague who thinks differently from you. But as a pre-flight check before you commit to a direction, they're more useful than the default mode of "tell me my idea is good."

## Try this: reviewer #2 stress test (10 min)

We now want to see whether AI might actually be able to provide some useful critique of your research. For that, intelligence matters (I'd hope). So make sure to use one of the best models available to you, whether that is the top option of a company you have subscribed to, or a recent leading open source model.

**Part 1: The stress test (5-7 min)**

Take your research question, abstract, or a brief project description - something you're currently working on.

Paste it into a chat LLM with this prompt (or your own version): "You are a skeptical senior reviewer who has seen too many papers making claims like this. Identify fatal flaws and fixable weaknesses in this research idea. Be specific."

Read the critique. Then write a brief human rebuttal for the top 3 points. Not a defensive rebuttal - a genuine response that either acknowledges the problem or explains why it isn't as bad as it sounds. (Bonus: Get the AI to assess it critically, and see what you make of that response.)

**Part 2: De-convergence protocol (pick one, 3-5 min)**

Try asking some of these about the piece of work you selected above (or another current project):

- "What assumption am I making here that I should think about again?"
- "Give me five rival hypotheses that would explain the same pattern without invoking [your main mechanism]."
- "What would be an unconventional approach to testing this idea?"

Notice whether the AI's critiques feel generic or specific to your work. The generic ones may be the convergence problem in action - the model reaching for standard objections rather than engaging with the specifics. The specific ones are where LLMs are more likely to add value.

**Journal prompt**

Where did AI help you think differently about your work? Where did it push you toward obvious, predictable critique? If you were to use AI for ideation regularly, what habits would you need to protect genuine originality?
