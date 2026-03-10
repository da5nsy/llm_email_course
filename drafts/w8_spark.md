**Subject:** [GAIR] Steering your AI research assistant

---

Week 8 of 10 - Agents for research workflows

---

Last week was about meeting agents and seeing what they can do. If you're like most people who try this for the first time, the experience was a mix of "that was impressive" and "that was wrong in a way I almost didn't notice." I certainly had (and still have) a mix of both reactions. This week is about making the impressive parts more reliable.

The difference between an ad hoc agent interaction and a useful one usually comes down to how well you specified the task. When you say "summarise these papers," you get _something_. When you say "extract these five specific pieces of information from each paper, flag anything you're uncertain about, and organise the result in a table I can verify row by row," you get something much better.

This isn't surprising. It's the same principle from Week 3: specificity helps. But with agents, specification matters more because the agent acts on your behalf across multiple steps. A vague prompt to a chat interface produces a vague response you can redirect. A vague prompt to an agent produces a series of actions you might not review individually. Most agents have a planning mode that helps to ensure you agree on a clear direction - but even there the initial prompt is key.

**Bounded tasks**

A bounded agent task has clear inputs, a defined output format, explicit acceptance criteria, and ideally a way to check whether it worked. The more of these you specify, the more reliable the result.

Think of it like briefing a research assistant. "Check whether my analysis is sound" is an open-ended task that could go anywhere. "Read my preregistration and analysis script, identify any place where they describe different procedures, list each discrepancy with line references, and assess which of the differences matter for validity" is bounded. You know what success looks like. You can check whether the assistant (human or AI) delivered it.

This doesn't mean every agent interaction needs a formal specification. For quick, low-stakes tasks - "rename these files according to this convention," "create a quick codebook that helps me understand this dataset" - a casual prompt is fine. There is little risk and you'll see immediately whether it worked. But for tasks where the output feeds into your research, where errors could propagate, or where verification is harder, the investment in specification pays off.

**The elements of a good spec**

When designing a bounded agent task, think about:

- *Inputs:* What exactly should the agent work with? Which files, which data, which documents? Be explicit. If you point an agent at a folder with 50 files but only want it to work with 10 of them, say so (or even better, curate the folder).
- *Output format:* What should the result look like? A table with specific columns? A written summary with section headers? Code that follows a particular structure? The more concrete the format, the easier it is to check.
- *Acceptance criteria:* How will you know if the output is good enough? "Every claim in the table must reference a specific page or section in the source document." "The code must run without errors on the sample dataset." "The summary must cover all five papers and not introduce claims from outside the provided sources."
- *Checkpoints:* For complex multi-step tasks, where should the agent pause and show you intermediate results? Catching a wrong turn after step 2 is cheaper than discovering it in the final output.
- *Failure modes:* What could go wrong? If the agent can't find information for a field, should it leave it blank, write "not found," or flag it for your review? Specifying this in advance prevents the agent from filling gaps with plausible-sounding fabrications.

You don't need to write a formal document for every task. But running through these questions in your head - or even in a few bullet points at the top of your prompt - makes a noticeable difference. This is also one place where web interfaces retain their place. Chatting through the plan with a conversational LLM can help find gaps.

**An example**

Here's what a bounded task might look like in practice. Say you're preparing a literature review and you have 8 papers on your desk.

A vague prompt: "Summarise these papers and identify the key themes."

A bounded version: "Read these 8 papers. For each one, extract: (1) the research question, (2) the method and sample size, (3) the main finding, (4) one key limitation the authors acknowledge, (5) one limitation they don't acknowledge but that I should consider. Present this in a table. If you're uncertain about any cell, mark it [UNCERTAIN] rather than guessing. Add highlights to any section of the PDFs that you cited. After the table, list 3 areas where the papers agree and 2 areas where they disagree, citing specific papers for each claim."

The second version takes two minutes longer to write, and will keep the agent busy for a bit longer. But it produces output you can actually verify cell by cell, it discourages fabrication, and it gives you a structured artefact you can build on. The first version produces a smooth summary that sounds great and is much harder to check ... and gives you a lot less to advance your own *thinking*.

**Iteration is part of the process**

Even with a good specification, the first output usually isn't quite right. A column might be interpreted differently from what you intended. The agent might focus on the wrong section of a paper. An acceptance criterion might turn out to be ambiguous.

Iteration is normal. The first run shows you where your specification was unclear, and you refine it. After two or three rounds, you typically have both a good output and a reusable specification you can apply to the next batch of papers, the next dataset, or the next project. That said, agent tasks are slower and more resource-hungry than a quick chat prompt, so it's worth building the habit of noting exactly what went wrong and why you expected it to go differently. That way, you quickly get better at specifying your intentions and requirements.

Iteration is also where agents differ most from chat. In a chat interface, each conversation starts fresh. With an agent that works in your project folder, you can save your specification as a file, refer back to it, and build on previous runs. Most agent tools also let you save a specification as a reusable *skill* or custom command - essentially a workflow you've refined that you can re-run with different inputs. With that, your specifications become reusable tools.

**Bounded tasks beyond literature**

The literature extraction example above is a possible starting point, but the same approach works for any research task. Here are a few worth trying:

- **Questionnaire assembly.**
  - Input: 3-5 papers that contain the scales you want to use, plus your study design notes.
  - Output: a compiled questionnaire with items extracted from each paper, source citations for every scale, and (if your survey tool supports it) an importable file such as a Qualtrics .qsf.
  - Acceptance criteria: every item traces back to a specific paper; no items invented; response formats match the originals.
- **Free-text coding.**
  - Input: a set of open-ended survey responses (or interview transcripts) and an initial coding template with definitions for each code.
  - Output: each response coded against the template, with the relevant passage quoted alongside each code assignment. Responses that don't fit any code flagged separately.
  - Acceptance criteria: codes are applied consistently with your definitions; flagged responses genuinely don't fit (not just ambiguous ones the agent skipped over).
- **Code generation.**
  - Input: your methods section or pre-registration, and an assumption regarding the effect size you are likely to find.
  - Output: well-documented analysis code, alongside a simulated dataset that can be used to check whether the code retrieves the expected effect size.
  - Acceptance criteria: code runs without errors, adheres to the analytical plan, and is cleanly documented.

In each case, the pattern is the same: define what goes in, what comes out, and how you'll check it.

## Try this: run a bounded agent project (10-15 min)

Pick one of the tasks above - or the literature extraction example - and run it with an agent (or extended chat session). You can refer to the literature example as a model for how detailed your specification should be.

1. Choose a task and gather your inputs (PDFs, a methods section, design parameters, or a pre-registration).
2. Write a specification: what should the agent extract or produce? What format? What should it do when uncertain?
3. Set at least one concrete acceptance criterion before you start.
4. Run it. Then check the output against your criteria and your own knowledge.
5. Note where your specification was too vague, and what you'd change next time.

**Journal prompt**

Did the agent do what you expected it to do? Did it meet your acceptance criteria? What would you change about your specification?