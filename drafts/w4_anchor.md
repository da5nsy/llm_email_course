**Subject:** [GAIR] Grounding helps retrieval, not judgment

---

Week 4 of 10 - Grounded tools: working with your own sources

---

If you tried the grounded synthesis test on Monday, you probably noticed two things. First, it felt different from chat. Claims came with citations. You could trace what the tool said back to specific passages. That's a real improvement over the floating assertions of a regular LLM.

Second, if you checked those citations carefully, you probably found at least one that didn't quite say what the tool claimed. A finding overstated. A caveat dropped. A conclusion presented without the qualifications the author actually attached to it.

Both observations matter, and they pull in opposite directions.

**Better at traceability, not at thinking**

Grounded tools are genuinely better than chat for anything involving specific claims or evidence. When the tool tells you "Smith et al. found X," you can check. That alone makes the generation-verification asymmetry from Week 2 work more in your favour: the tool generates a synthesis, and the source attribution makes your verification faster.

But the retrieval step - finding relevant passages in your documents - is only part of what research synthesis requires. The harder parts are weighting evidence (this well-powered RCT matters more than that convenience-sampled pilot), recognising when authors disagree about something important versus something minor, and noticing what's absent from the literature rather than what's present. Grounded tools don't do any of this well.

**The smoothing problem**

There's a specific failure mode worth watching for: homogenisation. When you ask a grounded tool to synthesise across several papers, it tends to produce something that reads like a consensus - even when the papers genuinely disagree. Conflicting findings get softened into "mixed results." Fundamentally different theoretical positions get presented as complementary perspectives. The output looks balanced and considered, but the actual tensions between sources have been filed down.

This is the convergence issue from last week showing up in a different form. The tool is optimised to produce coherent, readable summaries. Academic disagreement is messy and hard to summarise coherently. So it gets smoothed out.

This doesn't mean grounded tools are useless for synthesis. It means you need to read the output with a specific question in mind: "Is this telling me these sources agree, or is it making them sound like they agree?" If the answer matters for your work, go back to the originals on any point of claimed consensus.

**What about systematic reviews?**

Could grounded tools replace - or substantially assist - systematic or scoping reviews? They can help with specific steps: screening titles, extracting structured data from papers, identifying themes across a set of studies. But they can't replace the deliberate, documented search strategy that makes a review systematic. The tools don't expose their retrieval logic clearly enough, they miss papers for unpredictable reasons, and their synthesis doesn't meet the standards of transparency that systematic reviews require.

As aids within a structured workflow, they can save time. As substitutes for the workflow itself, they're not ready. [NEEDS CHECK: current state of AI-assisted systematic review tools - any newer tools designed specifically for this?]

## Try this: triangulation test (5-8 min)

Pick one paper you need to read for current work - something you haven't yet read in detail.

Ask a grounded tool (NotebookLM with the paper uploaded, or Elicit if the paper is in their corpus) for:

- 5 key claims the paper makes
- 3 areas of uncertainty or limitation the authors acknowledge
- 5 methodological details worth inspecting

Now spend 5 minutes with the actual paper: read the abstract, skim the figures and tables, glance at the discussion. Compare:

- What did the tool get right?
- What did it overstate or miss?
- Was there anything in the figures or tables that the tool couldn't access or interpret?

If you have time, try one more thing: ask a regular chat LLM (without the paper uploaded) the same questions about this paper. How different are the answers? That's the practical difference between grounded and ungrounded tools.

**Further exploration**

Compare the same research question across three sources: a regular chat LLM, a grounded tool, and a traditional database search (Google Scholar, PubMed, or your discipline's standard). What sources does each surface? Where's the overlap?

**Journal prompt**

How does the grounded tool's output compare to a good Wikipedia article or review paper on a topic you know? What's the difference in nuance, balance, and confidence? Where do you still need your own judgment most?
