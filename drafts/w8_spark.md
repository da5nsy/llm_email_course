**Subject:** [GAIR] From ad hoc to designed: bounded agent projects

---

Week 8 of 10 - Agents for research workflows

---

Last week was about meeting agents and seeing what they can do. If you're like most people who try this for the first time, the experience was a mix of "that was impressive" and "that was wrong in a way I almost didn't notice." Both reactions are correct. This week is about making the impressive parts more reliable.

The difference between an ad hoc agent interaction and a useful one usually comes down to how well you specified the task. When you say "summarise these papers," you get something. When you say "extract these five specific pieces of information from each paper, flag anything you're uncertain about, and organise the result in a table I can verify row by row," you get something much better.

This isn't surprising. It's the same principle from Week 3: specificity helps. But with agents, specification matters more because the agent acts on your behalf across multiple steps. A vague prompt to a chat interface produces a vague response you can redirect. A vague prompt to an agent produces a series of actions you might not review individually.

**Bounded tasks**

A bounded agent task has clear inputs, a defined output format, explicit acceptance criteria, and ideally a way to check whether it worked. The more of these you specify, the more reliable the result.

Think of it like briefing a research assistant. "Look into the literature on X" is an open-ended task that could go anywhere. "Find the 5 most-cited empirical papers on X published since 2020, and for each one extract: the sample size, the primary outcome measure, the main finding, and one stated limitation" is bounded. You know what success looks like. You can check whether the assistant (human or AI) delivered it.

This doesn't mean every agent interaction needs a formal specification. For quick, low-stakes tasks - "rename these files according to this convention," "clean up the formatting in this document" - a casual prompt is fine. The stakes are low and you'll see immediately whether it worked. But for tasks where the output feeds into your research, where errors could propagate, or where verification is harder, the investment in specification pays off.

**The elements of a good spec**

When designing a bounded agent task, think about:

- **Inputs:** What exactly should the agent work with? Which files, which data, which documents? Be explicit. If you point an agent at a folder with 50 files but only want it to work with 10 of them, say so.
- **Output format:** What should the result look like? A table with specific columns? A written summary with section headers? Code that follows a particular structure? The more concrete the format, the easier it is to check.
- **Acceptance criteria:** How will you know if the output is good enough? "Every claim in the table must reference a specific page or section in the source document." "The code must run without errors on the sample dataset." "The summary must cover all five papers and not introduce claims from outside the provided sources."
- **Failure modes:** What could go wrong? If the agent can't find information for a field, should it leave it blank, write "not found," or flag it for your review? Specifying this in advance prevents the agent from filling gaps with plausible-sounding fabrications.

You don't need to write a formal document for every task. But running through these questions in your head - or even in a few bullet points at the top of your prompt - makes a noticeable difference.

**An example**

Here's what a bounded task might look like in practice. Say you're preparing a literature review and you have 8 papers on your desk.

A vague prompt: "Summarise these papers and identify the key themes."

A bounded version: "Read these 8 papers. For each one, extract: (1) the research question, (2) the method and sample size, (3) the main finding, (4) one key limitation the authors acknowledge, (5) one limitation they don't acknowledge but that I should consider. Present this in a table. If you're uncertain about any cell, mark it [UNCERTAIN] rather than guessing. After the table, list 3 areas where the papers agree and 2 areas where they disagree, citing specific papers for each claim."

The second version takes two minutes longer to write. But it produces output you can actually verify cell by cell, it discourages fabrication, and it gives you a structured artefact you can build on. The first version produces a smooth summary that sounds great and is much harder to check.

**Iteration is part of the process**

Even with a good specification, the first output usually isn't quite right. A column might be interpreted differently from what you intended. The agent might focus on the wrong section of a paper. An acceptance criterion might turn out to be ambiguous.

This is normal, not a failure. The first run shows you where your specification was unclear, and you refine it. After two or three rounds, you typically have both a good output and a reusable specification you can apply to the next batch of papers, the next dataset, or the next project.

This is also where agents differ most from chat. In a chat interface, each conversation starts fresh. With an agent that works in your project folder, you can save your specification as a file, refer back to it, and build on previous runs. Your specifications become reusable tools.

**Beyond literature: other bounded tasks**

The literature extraction example is common because it's familiar, but the same approach works for other research tasks:

- **Methodology critique:** Input: your methods section or study design. Output: structured critique identifying assumptions, threats to validity, and suggestions, each tied to a specific part of your design. Acceptance criteria: identifies at least 2 issues you agree with and explains why they matter.
- **Materials generation:** Input: study design parameters and constraints. Output: draft materials (survey items, interview protocols, vignettes for stimulus sampling). Acceptance criteria: materials match your specified constraints, nothing is fabricated, and each item can be traced to a design requirement.
- **Data documentation:** Input: a dataset and any existing documentation. Output: a codebook or data dictionary describing each variable, its type, its range, and any apparent coding conventions. Acceptance criteria: descriptions match the actual data, and unknowns are flagged rather than guessed.

In each case, the pattern is the same. Define what goes in, what comes out, and how you'll check it.

## Try this: design and run one bounded agent project (10-15 min)

Choose one of the tasks below (or adapt one to your current work) and run it with an agent or extended chat session.

**Option A - Literature extraction table:**
- Gather 3-5 PDFs relevant to a current project.
- Write a specification: what to extract from each paper (e.g., research question, method, sample size, main finding, key limitation, your confidence in the AI's extraction).
- Set acceptance criteria: every claim must have a page/section pointer, or be marked "needs verification."
- Run it. Check the output against the actual papers.

**Option B - Methodology critique:**
- Take your methods section or a brief description of your study design.
- Ask the agent to produce a structured critique: assumptions, threats to validity, missing details, and suggestions.
- Set acceptance criteria: the critique must identify at least 2 issues you agree are real problems.
- Assess: did it find things you'd missed? Did it flag things that aren't actually problems?

**Option C - Materials generation:**
- Define parameters for study materials you need (e.g., "5 vignettes varying [factor] across [levels], each 100-150 words, written in [register]").
- Set acceptance criteria: materials match the constraints, nothing is fabricated, tone is consistent.
- Review: do the materials actually vary the factor you specified? Are they usable as-is, or do they need substantial editing?

Whichever you choose, pay attention to your specification. Was it detailed enough? Where did ambiguity cause problems? What would you change for next time?

**Journal prompt**

What acceptance criteria did you set? Did the agent meet them? What would you change about your specification?
