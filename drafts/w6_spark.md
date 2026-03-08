**Subject:** [GAIR] Let it write your code, then check everything

---

Week 6 of 10 - AI for coding and data

---

For five weeks, you've been working with text. Prompts, summaries, critiques, writing. This week is about data and code.

If you already write code - R, Python, Stata - AI has probably already changed how you work. You describe an analysis, get code back, paste it into your environment, and iterate. This email is partly about making that workflow more deliberate.

If you don't write code, this week is an invitation to try. AI has lowered the barrier enough that you can get useful scripts running with no prior programming experience. You describe what you want in plain language, get working code, and run it. You don't need to understand every line - but you do need to understand the output well enough to know whether it's right. That's a skill you already have: it's called being a researcher.

Either way, this week is optional in the sense that the remaining weeks don't require it. If coding isn't relevant to your work and you'd rather skip ahead, you can. But if you've ever thought "I know what analysis I need, I just can't write the code" - this is a good week to experiment.

**AI writes code now**

Here's the basic idea. You open a chat LLM - ChatGPT, Claude, Gemini, whatever you use - and describe what you need. "Write me R code to run a mixed-effects model predicting Y from X1 and X2, with random intercepts for participant." Or "Write a Python script that cleans this CSV: recode these variables, drop incomplete rows, and export a summary table." The AI produces code. You paste it into RStudio, or a Jupyter notebook, or whatever environment you work in. You run it.

If you don't have a coding environment set up, you can use browser-based tools instead. ChatGPT's code interpreter, Claude's artifacts, and Google Colab all let you upload data and run code without installing anything. They're more limited than a local setup, but for getting started they work well.

[NEEDS CHECK: current state of these tools - which are free, which require paid plans, any significant new options]

**The copy-paste loop**

In practice, it rarely works on the first try.

You describe your analysis. The AI writes code. You paste it into your environment - and get an error. Maybe a package isn't installed. Maybe the variable names don't match your dataset. Maybe the AI assumed your data was in long format when it's wide. So you copy the error message, paste it back into the chat, and the AI tries again. Maybe it works now. Maybe there's a different error. You provide more detail about your data. The AI adjusts. Eventually, something runs.

This is the copy-paste loop: chat window on one side, IDE on the other, you in the middle shuttling code and error messages back and forth. It works surprisingly often for getting from "I have data" to "I have results." It also gets tedious. And it's worth noticing what's happening cognitively: you're spending your attention on managing the interaction rather than thinking about the analysis. Whether that trade-off is worth it depends on the task. For a quick descriptive table, absolutely. For a complex analysis where modelling choices matter, probably less so.

We'll come back to the friction of this workflow. There are tools that eliminate it, and we'll get to those.

**Code that runs is not code that's right**

This is the most important thing to understand about AI-generated code, whether you're a programmer or not: code can execute without errors and produce results that look entirely plausible but are wrong.

The AI reverses a scale, so your positive correlation becomes negative. It drops rows with missing data without mentioning it, changing your sample size by 15%. It runs a t-test when your design calls for a paired comparison. It generates a clean visualisation with mislabelled axes. It recodes a categorical variable and silently merges two categories that shouldn't be combined. Each of these will produce output. None will throw an error.

[ADD PERSONAL EXPERIENCE: specific examples of AI code that ran but was wrong]

What catches these mistakes isn't programming expertise. It's domain knowledge. You know that a negative correlation between these two variables doesn't make theoretical sense in your field. You know your sample should be 450, not 380. You know the groups aren't independent. You know that "strongly agree" is 5, not 1. The AI doesn't know any of this unless you tell it, and even when you do, it might not flag the problem.

This is why the exercise includes verification steps. Running the code is half the job. Checking whether the output makes substantive sense is the other half. The good news is that AI also makes verification easier: you can ask it to produce summary statistics, check sample sizes, and create diagnostic plots. The bad news is that you need to know which checks to ask for, and that knowledge comes from your training as a researcher, not from the tool.

**A note on data privacy**

Before sharing any data with an AI tool, think about what's in the file. When you paste data into a chat interface or upload it to a browser tool, it's processed on remote servers, and some providers use uploaded content for model training unless you opt out. Anonymised or public datasets are usually straightforward. Participant-level data with identifiers needs more care. Check whether your institution's data governance policies allow cloud-based processing, and whether the specific tool you're using stores or trains on uploaded data.

## Try this: AI-assisted data analysis (10-15 min)

1. Take a dataset you're working with, or grab a public one (e.g., from the [General Social Survey](https://gss.norc.org/), [Our World in Data](https://ourworldindata.org/), or another source in your field).
2. Ask a chat LLM to write code for a specific analysis: "Write R/Python code to explore the relationship between X and Y, controlling for Z" or "Write code to show the distribution of [variable] across [groups]." If you don't normally write code, R is a good starting point for social science data - ask the AI to include installation instructions for any packages it uses.
3. Run the code in your environment. If you don't have one set up, upload the data to ChatGPT's code interpreter or Claude and let it run the analysis in the browser.
4. Iterate: when you get errors, paste them back into the chat. When you get output, check it against what you'd expect.
5. Sanity check: Are the sample sizes right? Are the scales in the right direction? Do the descriptive statistics match what you'd expect from eyeballing the data?

Pay attention to the workflow itself. How much time did you spend shuttling between chat and your editor versus thinking about your research question? When errors came up, did the AI's fix actually solve the problem or introduce new ones?

**Journal prompt**

What did the AI get right that would have taken you a while? What did it get wrong that you almost missed? How did the copy-paste workflow feel?
