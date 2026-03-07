**Subject:** [GAIR] When cheap iteration becomes a confound

---

Week 6 of 10 - AI for coding and data: in the browser

---

If you ran the browser analysis on Monday, you probably noticed how easy it was to try different approaches. Change a variable, rerun. Ask for a different visualisation, get one in seconds. Try a different statistical test, see what happens. The effort required for each alternative was close to zero.

That ease is today's topic. Because it has consequences that aren't obvious in the moment.

**Forking paths**

In any data analysis, you make choices. Which observations to include. How to code a variable. What covariates to control for. Which statistical test to use. Each choice is reasonable on its own, but each one is also a fork in the path. Take enough forks and you can arrive at almost any destination.

This is the garden of forking paths problem, and it's not new. Researchers have been navigating these choices forever. What *is* new is the speed. AI makes it trivially easy to try dozens of alternatives in minutes. Upload data, ask for one analysis, look at the results, ask for another. Each iteration takes seconds.

The temptation to keep going until something "works" is real, even when you're not consciously looking for a particular result. You try several specifications, one produces a significant effect, and you write up that one because it seemed most interesting. The problem is that you've just run a high-throughput search through your analytic options without adjusting for the number of comparisons. The false positive rate is quietly inflated. This isn't p-hacking in the deliberate sense. It's undisciplined exploration, and AI makes it frictionless.

**Pre-commitment as discipline**

The antidote is boring but effective: decide your primary analysis before running alternatives.

This doesn't mean you can't explore. Exploratory analysis is legitimate and valuable. But there's a difference between exploration and confirmation, and the line between them needs to be drawn before you see the results. Write down your primary analysis plan in one sentence before you start iterating: "Primary analysis will be [X]. Exploratory analyses will be labelled as such."

If you're in a field where pre-registration is common, AI actually strengthens the case for it. When the cost of running alternatives is nearly zero, the discipline of committing in advance becomes more important, not less.

**Broken legs checks**

Before running any substantive analysis, there are cheap sanity checks that catch obvious problems. Check for impossible values (ages of 900, negative response times). Look for coding inversions (did the AI flip your Likert scale when it recoded the data?). Examine missingness patterns (did it silently drop observations?). Verify that group sizes match what you expected.

These checks take minutes and prevent hours of wasted analysis on corrupted data. The name comes from actuarial science: if your statistical model predicts someone will live to 100 but they have a broken leg, maybe update the prediction. Simple information that overrides complex models.

AI is actually good at generating these checks for you. Ask it: "Before we run the main analysis, list sanity checks I should run on this dataset." It will typically produce a reasonable list. The irony is that the tool most likely to introduce data problems is also quite good at suggesting how to catch them.

**The friction you just felt**

If you worked through Monday's exercise, there's one more thing worth noticing. The copy-paste workflow - uploading data, describing what you want, pasting errors back, manually copying results - involves a lot of friction. You're spending cognitive effort on managing the interaction rather than thinking about your research question.

That friction is the problem that the next generation of AI tools is designed to address. Agents can access files, run code, handle errors, and iterate autonomously without you pasting things back and forth. Whether that's a net gain depends on how much of the friction was also serving as a natural checkpoint, forcing you to inspect intermediate results. We'll get to that.

If you need a breather, this is a natural place to pause. The first six weeks have covered a lot of ground, and it's worth letting the skills settle before adding more. But do come back: the second half of the course tackles questions about agents, governance, and institutional strategy that matter whether or not you personally adopt every tool we've discussed.

## Try this: pre-commitment exercise (8-10 min)

1. Take an analysis you've already run, or one you're planning to run soon.
2. Ask a chat LLM: "I'm planning to analyse [brief description of your research question and data]. List all the reasonable analytic choices I'll need to make - variable coding, exclusion criteria, statistical tests, covariates, and anything else that could vary."
3. Read the list. It will probably be longer than you expected. Each item is a fork in the path.
4. Pick one primary analysis plan and write a one-sentence pre-commitment: "Primary analysis will be [specific approach] unless [specific predefined condition], in which case [specific alternative]."

**Further exploration:** Try the multimodal extraction exercise. Screenshot a table or chart from a PDF, upload the screenshot to a chat LLM, and ask it to transcribe the data into a CSV. Then spot-check 5 random cells against the original. This is a high-return use case wherever verification is cheap and manual data entry is tedious.

**Journal prompt**

How many analytic choices did the AI surface that you hadn't considered? How does that change your thinking about pre-registration?
