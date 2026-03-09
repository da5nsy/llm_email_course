**Subject:** [GAIR] When cheap iteration becomes a risk

---

Week 6 of 10 - AI for coding and data

---

If you tried Monday's exercise, you probably noticed something beyond the copy-paste friction: trying different approaches was remarkably easy. Change a variable, ask for new code, run it. Try a different statistical test, see what happens. Request a different visualisation. Each alternative costs almost nothing.

On Monday, the focus was on whether any single analysis is correct: silent errors, wrong scales, dropped observations. Today is about a different problem. Even when each analysis is individually right, running many of them and reporting the most interesting one introduces bias. And AI makes running many of them very, very easy.

**Forking paths**

In any data analysis, you make choices. Which observations to include. How to code a variable. What covariates to control for. Which statistical test to use. Each choice is reasonable on its own, but each one is also a fork in the path. Take enough forks and you can arrive at almost any destination.

This is the garden of forking paths problem, and it's not new. Researchers have been navigating analytic choices forever. What *is* new is the speed. AI makes it trivially easy to try dozens of specifications in minutes. You try several, one produces a significant effect, and you write that one up because it seemed most interesting. The problem is that you've searched through your analytic options without accounting for how many you tried. This isn't *p*-hacking in the deliberate sense (that is actually something many AI models actively resist). It's undisciplined exploration, and AI makes it frictionless.

On Monday, we also noted a related risk: if you prompt the AI to find support for a hypothesis rather than write open-ended analysis code, the model itself may make choices that push toward the result you asked for. So the bias can come from two directions: your selection of which results to report, and the AI's tendency to give you what you asked for.

**Pre-commitment as discipline**

The antidote is boring but effective (and needed not only if you use AI): decide your primary analysis before running alternatives.

This doesn't mean you can't explore. Exploratory analysis is legitimate and valuable. But there's a difference between exploration and confirmation, and the line between them needs to be drawn before you see the results. Write down your primary analysis plan before you start iterating. Label exploratory analyses as such.

Pre-registration is becoming increasingly common across fields - and even if it is still novel in your field, there is little downside to it. AI clearly strengthens the case for it. When the cost of running alternatives is nearly zero, the discipline of committing in advance becomes more important. And AI can help here: you can ask it to identify all the analytic choices in your design (see the exercise below), to simulate data, and to draft analysis code. A thorough list of decision points is halfway to a pre-registration. Working code tested against simulated data makes it more credible and practical still.

**Keep a log**

One practical habit worth building: when you're iterating with AI, keep a brief record of what you tried and why. Your chat history captures the code, but not your reasoning. A few lines in a text file ("tried controlling for age, effect disappeared, decided to keep it as primary because [reason]") make the difference between transparent exploration and a fishing expedition. It also makes methods sections much easier to write.

## Try this: map your analytic choices (5-8 min)

1. Take an analysis you've already run, or one you're planning.
2. Ask a chat LLM: "I'm planning to analyse [brief description of your research question and data]. List all the reasonable analytic choices I'll need to make - variable coding, exclusion criteria, statistical tests, covariates, and anything else that could vary."
3. Read the list. It will probably be longer than you expected. Each item is a fork in the path - though some might not actually be plausible choices, theoretically or because of conventions in your discipline.
4. Pick one primary analysis plan and write a one-sentence pre-commitment: "Primary analysis will be [specific approach] unless [specific predefined condition], in which case [specific alternative]."

**Journal prompt**

How many analytic choices did the AI surface that you hadn't considered? Does that change your thinking about pre-registration?
