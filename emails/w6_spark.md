**Subject:** [GAIR] Let it write your code, then check everything

---

Week 6 of 10 - AI for coding and data

---

You're halfway through the course. The first five weeks were about text: understanding LLMs, prompting, grounded tools, writing. The second half is more about getting AI to *do* things, starting now with data and code, then moving to agents and governance.

If you've ever been annoyed at clicking through SPSS menus again because one pre-processing step changed, or wished you could share your exact analysis steps with a collaborator, code is the answer. And AI has made getting started with code dramatically easier. You describe what you want in plain language, the AI writes the code, and you run it. You don't need to understand every line, but you do need to understand the output well enough to know whether it's right. If you run into trouble, you can paste the error back and ask the AI to fix it, or ask it to explain what the code does.

If you already write code in R, Python, or Stata, AI has likely changed how you work already. This email is about making that workflow more deliberate, and about the verification habits that matter regardless of your experience level.

**The workflow**

You open a chat LLM and describe what you need. "Write R code to run a mixed-effects model predicting Y from X1 and X2, with random intercepts for participant." Or "Write a Python script that cleans this CSV: recode these variables, drop incomplete rows, and export a summary table." The AI produces code. You paste it into RStudio, or a Jupyter notebook, or whatever environment you work in. You run it.

If you don't have a coding environment set up, [Google Colab](https://colab.research.google.com/) lets you run code in the cloud without installing anything. It's a solid way to get started.

**Why code, not just "analyse this"?**

You can upload a dataset to ChatGPT's code interpreter and just say "analyse this." Some tools will produce entire reports from a single prompt. For a quick first look at unfamiliar data, that's useful: upload a CSV, ask "what's in here?", and get summary statistics and plots in minutes.

But for anything you'd put in a paper, it's worth seeing (and saving) the code. When the AI runs analysis behind the scenes and shows you polished output, you can't tell what choices it made. Did it drop missing values or impute them? How did it code that variable? Which observations did it include? You get a clean-looking result with no way to inspect the path that produced it - and in extreme cases, AI might even hallucinate in code. The first time I used ChatGPT Code Interpreter, it invented and hard-coded a correlation value to get us over the line. This has become very rare, but can still occur.

Code gives you a record. Even if you didn't write it, even if you don't entirely understand it, you can read through and see that on line 12 it filtered out participants under 18, and on line 15 it reverse-coded items 3 and 7. You can share that with a collaborator or reviewer (or even another LLM for a second critical look). You can run it again on updated data and get consistent results. That transparency is why code matters for research, and why learning to at least *read* code is worth the investment, even if AI writes most of it for you.

**The copy-paste loop**

In practice, code rarely works on the first try. Not because AI makes frequent errors, but because something is specific to your setup, or a detail of the analysis was ambiguous until you tried it. This gives rise to a cycle: you paste the code into your environment, get an error, copy the error message back into the chat, get revised code, try again. Chat window on one side, editor on the other, you in the middle shuttling code and errors back and forth.

This works surprisingly often for getting from "I have data" to "I have results." It also gets tedious. As you get more comfortable reading code, you'll start noticing fixes you could make directly: a typo in a variable name, a wrong file path. Sometimes just fixing the line yourself is faster and teaches you more, but I have certainly found myself getting stuck in the pattern of copying and pasting, rather than thinking, which is obviously not ideal.

We'll come back to the inefficiencies in that workflow. There are tools that reduce it substantially, and we'll get to those next week. Now, there is something more fundamental to address.

**Code that runs is not code that's right**

This is the most important point in this email: AI-generated code can execute without errors and produce results that look entirely plausible but are wrong.

The AI might include a missing value indicator (-99) in calculating a mean. Or treat a categorical variable as continuous, or drop rows with missing data so that your sample size quietly changes between analyses. It might run a t-test when your design calls for a paired comparison. Or generate a clean visualisation with mislabelled axes.

You can sometimes spot these by reading the code, and programming expertise helps. But domain knowledge matters more. You know that a negative correlation between these two variables doesn't make theoretical sense. You know your sample should be 450, not 380. You know the groups aren't independent. You know that "strongly agree" is 5, not 1. The AI doesn't know any of this unless you tell it (or you upload good data documentation).

Generating and running the code is half the job. Checking whether the output makes substantive sense is the other half. AI can help here too: ask it to produce summary statistics, check sample sizes, and create diagnostic plots. But you need to know which checks to ask for, and that knowledge comes from your training as a researcher, not from the tool.

**A note on data privacy**

Before sharing data with an AI tool, think about what's in the file. When you paste data into a chat or upload it to a browser tool, it's processed on remote servers, and some providers use uploaded content for model training unless you opt out. Anonymised or public datasets are usually straightforward. Participant-level data with identifiers needs more care. Check your institution's data governance policies and the specific tool's data handling practices.

## Try this: AI-assisted data analysis (10-15 min)

This week is optional in the sense that the remaining weeks don't build on it directly. But if code-based analysis is even slightly relevant to your work, it's worth experimenting.

1. Take a dataset you're working with, or grab a public one (e.g., from the [General Social Survey](https://gss.norc.org/), [Harvard Dataverse](https://dataverse.harvard.edu/), or another source in your field).
2. Ask a chat LLM to write code for a specific analysis: "Write R/Python code to explore the relationship between X and Y, controlling for Z" or "Write code to show the distribution of [variable] across [groups]." If you don't normally write code, R is a good starting point for social science data. Ask the AI to include installation instructions for any packages it uses.
3. Run the code in your environment. If you don't have a local setup, [Google Colab](https://colab.research.google.com/) lets you run code notebooks in the cloud.
4. Iterate: when you get errors, paste them back into the chat. When you get output, check it against what you'd expect.
5. Sanity check: Are the sample sizes right? Are the scales in the right direction? Do the descriptive statistics match what you'd expect from eyeballing the data?

Think about how much context helps. If the model has your codebook and analysis plan, it will write better code than if you just describe the dataset vaguely. But beware of putting too much pressure onto the model. The risk of hallucinations and questionable choices increases if the model is tasked with finding support for your hypothesis, rather than with generating open-ended analysis code.

**Journal prompt**

What did the AI get right that would have taken you a while? What did it get wrong that you almost missed? How did the copy-paste workflow feel?
