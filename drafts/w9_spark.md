**Subject:** [GAIR] The policies that already govern you

---

Week 9 of 10 - Governance and disclosure

---

You finish a paper. You go to submit. The journal asks: "Was AI used in the preparation of this manuscript? If so, please provide a statement describing how it was used."

You used Claude to restructure your discussion section. ChatGPT debugged your analysis code. An agent extracted data from 15 PDFs. You asked Gemini for feedback on your abstract. What do you write?

If you're not sure, you're not alone. The rules governing AI use in research are clearer than they were a year ago, but they're still patchy, sometimes contradictory, and often more specific than researchers expect. This week is about knowing what applies to you and building habits that keep you on the right side of whatever policies come next.

**What publishers require**

Most major publishers have converged on a few principles:

- AI cannot be listed as an author. It can't take responsibility for the work, so authorship doesn't apply.
- You must disclose AI use, typically in a dedicated methods statement or acknowledgments section.
- Human authors bear full responsibility for accuracy, integrity, and originality - including anything AI helped produce.

Documentation standards are getting more specific. Best practice is moving toward specifying: which tool (name and version), when, for what task, and which parts of the manuscript were affected. "I used ChatGPT for editing" is too vague to be useful to anyone. "I used Claude 3.5 Sonnet (October 2024) to suggest structural revisions to the Discussion, which I then substantially rewrote" gives a reader something to work with.

Check your target journals before you submit. Nature, Science, and most Elsevier and Springer journals have explicit policies. Many are broadly similar, but some have specific requirements about what counts as adequate disclosure. If you publish across disciplines, you may need to satisfy different standards for the same paper. The habit of checking matters more than memorising current rules, because these policies are still evolving.

**Your institution, funder, and professional body**

Journals aren't the only ones with policies. Your university likely has guidance on AI use in research, though the detail varies enormously. Some institutions have issued comprehensive frameworks; others are silent, which doesn't mean anything goes. It usually means policy hasn't caught up with practice.

Funders are moving more slowly, but some have started requiring disclosure or setting boundaries on how AI is used in grant-funded work. Professional bodies in your field may have their own guidelines too. Check your grant terms and your association's ethics code.

The practical headache is that these policies don't always align. A journal might require disclosure that your institutional guidance doesn't mention. A funder might restrict AI use in ways a journal doesn't care about. When in doubt, more transparency is safer. Nobody has been penalised for over-disclosing their AI use. The same is not true for under-disclosing.

**The collaborator problem**

Here's something the formal policies often miss: what happens when you use AI on shared work?

I recently heard about a researcher who discovered that a collaborator had been using an AI coding agent to make contributions to their shared GitHub repository. The commits arrived with a "Co-Authored-By: Claude" tag in the commit history - something the contributor hadn't mentioned or discussed. The code was fine. The problem was that nobody had agreed to AI contributions in a shared project, and one researcher was now associated with AI-assisted work they hadn't consented to.

This kind of situation is going to come up more. If you're working on a shared paper, a joint dataset, or a collaborative codebase, your AI use affects your collaborators. They may have different views on AI, different institutional requirements, or different comfort levels with disclosure. Using AI on collaborative work without discussion is a bit like bringing an undisclosed research assistant onto a project - the work might be good, but the process matters.

The practical fix is straightforward: have the conversation before it becomes a problem. It doesn't need to be a formal agreement, though for large projects it probably should be. At minimum: "I'm planning to use [tool] for [task]. Are you comfortable with that? How should we disclose it?" If AI contributions end up in shared outputs, everyone involved should know and agree. This is especially important when AI use might be visible to others - co-author tags in version control, stylistic tells in writing, or metadata that tools sometimes embed in files.

**Privacy: a brief reminder**

We covered data handling in Week 7 - what leaves your machine when you use an agent, cloud vs local processing, the difference between open and closed models. The same principles apply here. One thing worth adding: free tools often have weaker data protections than paid ones. Some free tiers explicitly reserve the right to use your inputs for training. If your data requires ethics approval, check the provider's terms before uploading it.

**Resource proportionality**

A quick practical point. You don't need to send everything to the most powerful available model. A grammar check doesn't need a frontier model. Routine formatting doesn't need an agent. Using smaller, cheaper, and where possible local tools for small tasks is partly about cost, partly about data exposure, and partly about not reaching for the most resource-hungry option by default. Match the tool to the task.

## Try this: policy hunt + disclosure draft (10-15 min)

1. Locate the AI use policies that apply to your work. Check: your institution's research guidelines, your funder (if applicable), two journals you might submit to, and your professional body (e.g., APA, BSA, APSA).
2. For each, note: what's explicitly required? What's ambiguous? What's not addressed at all?
3. Draft a brief AI disclosure statement suitable for your next paper. Be specific: name the tools, the tasks, the sections affected.
4. If you currently work with collaborators, draft a short "AI use agreement" you could propose to the team. What would you want to know about a collaborator's AI use? What would you want them to know about yours?

**Journal prompt**

Where are your personal red lines now compared to Week 1? What's shifted? What would you need to see in a collaborator's AI disclosure to feel comfortable?
