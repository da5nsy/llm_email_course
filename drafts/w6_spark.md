**Subject:** [GAIR] Let it write your code, then check everything

---

Week 6 of 10 - AI for coding and data: in the browser

---

For five weeks, you've been working with text. Prompts, summaries, critiques, writing. This week is about data.

Whether you write code regularly or haven't touched a script since that one stats course, AI has changed what's possible without leaving your browser. And that shift matters more than it might sound, because it means that data tasks which used to require software setup and programming knowledge can now be done by describing what you want in plain language.

**Browser-based coding tools**

Several tools now let you write and run code directly in a browser window, with AI doing most of the writing.

**ChatGPT** (on paid plans) has a code interpreter that runs Python in a sandboxed environment. You upload a file, describe what you want, and it writes and executes code for you. **Claude** can create interactive visualisations and run analysis through its artifacts feature. **Google Colab** gives you a notebook environment where you can pair AI assistance with executable code cells. There are others appearing regularly.

[NEEDS CHECK: current state of these tools - which are free, which require paid plans, any significant new options]

The common thread: none of these require you to install anything on your computer. You upload your data, describe what you want in words, and iterate from there. For researchers who don't code, this drops the barrier to entry substantially. For those who do, it speeds up the tedious parts.

**Two tracks**

"Data work" means different things to different researchers, so this week's exercise has two tracks.

If you work with quantitative data - surveys, experiments, observational datasets - there's a track that involves uploading data and running analysis. If your data work is more about text processing - cleaning reference lists, extracting information from tables, reformatting messy files - there's a track for that. Both are real research tasks that eat real hours. Both benefit from AI in similar ways, and both have similar failure modes. Pick whichever fits your work, or try both if you have time.

**The copy-paste loop**

Here's what the workflow actually looks like in practice.

You upload your data. You describe what you want: "Show me the distribution of responses by age group" or "Reformat this reference list from Vancouver to APA style." The AI writes code (or processes the text directly). Sometimes it works on the first try. Often it doesn't.

You get an error message. You paste it back in. The AI tries again. Maybe it works now. Maybe there's a different error. You describe the problem in more detail. The AI adjusts. Eventually, something runs. You look at the output and decide whether it's what you wanted, or whether you need another round.

This is the copy-paste loop. If you try the exercise below, you'll experience it first-hand. It works surprisingly often for getting from "I have data" to "I have a result." It also gets tedious. And it's worth noticing what's happening cognitively: you're spending your attention on managing the tool rather than thinking about the analysis. Whether that trade-off is worth it depends on the task. For a quick descriptive table, absolutely. For a complex analysis that requires judgment about modelling choices, maybe less so.

**Code that runs is not code that's right**

This is the most important thing to understand about AI-generated code, whether you're a programmer or not: code can execute without errors and produce results that look entirely plausible but are wrong.

The AI reverses a scale, so your positive correlation becomes negative. It drops rows with missing data without mentioning it, changing your sample size by 15%. It runs a t-test when your design calls for a paired comparison. It generates a clean visualisation with mislabelled axes. It recodes a categorical variable and silently merges two categories that shouldn't be combined. Each of these will produce output. None will throw an error.

[ADD PERSONAL EXPERIENCE: specific examples of AI code that ran but was wrong]

What catches these mistakes isn't programming expertise. It's domain knowledge. You know that a negative correlation between these two variables doesn't make theoretical sense in your field. You know your sample should be 450, not 380. You know the groups aren't independent. You know that "strongly agree" is 5, not 1. The AI doesn't know any of this unless you tell it, and even when you do, it might not flag the problem.

This is why the exercise includes verification steps. Running the code is half the job. Checking whether the output makes substantive sense is the other half. The good news is that AI also makes verification easier: you can ask it to produce summary statistics, check sample sizes, and create diagnostic plots. The bad news is that you need to know which checks to ask for, and that knowledge comes from your training as a researcher, not from the tool.

**A note on data privacy**

Before uploading any data to a browser-based AI tool, think about what's in the file. Many tools process data on remote servers, and some use uploaded content for model training unless you opt out. Anonymised or public datasets are usually straightforward. Participant-level data with identifiers needs more care. Check whether your institution's data governance policies allow cloud-based processing, and whether the specific tool you're using stores or trains on uploaded data.

## Try this: browser data analysis (10-15 min)

Pick one track and follow it through. If you have time, try both.

**Quant track:**

1. Take a dataset you're working with, or grab a public one (e.g., from the [General Social Survey](https://gss.norc.org/), [Our World in Data](https://ourworldindata.org/), or another source in your field).
2. Upload it to **ChatGPT** (code interpreter), **Claude**, or a **Google Colab** notebook.
3. Ask a specific analysis question: "Explore the relationship between X and Y, controlling for Z" or "Show me the distribution of [variable] across [groups]."
4. Iterate: when it produces errors, paste them back. When it produces output, check it against what you'd expect.
5. Sanity check: Are the sample sizes right? Are the scales in the right direction? Do the descriptive statistics match what you'd expect from eyeballing the data?

**Text processing track:**

1. Take a messy data task you've been putting off: reformatting a reference list between citation styles, extracting data from a table in a PDF, cleaning inconsistent variable names or coding schemes.
2. Upload the file to a browser-based AI tool.
3. Ask it to process the data with specific output requirements ("Convert to APA 7th edition" or "Output as a CSV with columns for author, year, title, journal").
4. Spot-check at least 5 entries against the original. Note what it got right and what it changed or dropped.

Whichever track you choose, pay attention to the workflow itself. How much time did you spend describing what you wanted versus checking what you got? When errors came up, did the AI's fix actually solve the problem or introduce new ones?

**Journal prompt**

What did the AI get right that would have taken you a while? What did it get wrong that you almost missed? How did the copy-paste workflow feel?
