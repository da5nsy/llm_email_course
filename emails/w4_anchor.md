**Subject:** [GAIR] Grounding helps retrieval, not judgment

---

Week 4 of 10 - Grounded tools: working with your own sources

---

Grounded tools feel different from chat. Claims come with citations. You can trace what the tool says back to specific passages. That's a real improvement over the floating assertions of a regular LLM.

But if you checked those citations carefully on Monday, you probably found at least one that didn't quite say what the tool claimed. A finding overstated. A caveat dropped. A conclusion presented without the qualifications the author actually attached to it.

Both observations matter, and they pull in opposite directions.

**Better at traceability, not at thinking**

Grounded tools are better than chat for anything involving specific claims or evidence. When the tool tells you "Smith et al. found X," you can check. That alone makes the generation-verification asymmetry from Week 2 work more in your favour: the tool generates a synthesis, and the source attribution makes your verification faster.

But the retrieval step - finding relevant passages in your documents - is only part of what research synthesis requires. The harder parts are weighting evidence, recognising when authors disagree about something important versus something minor, and noticing what's absent from the literature rather than what's present. Grounded tools are getting better at all of this as the foundational LLMs that power them improve - but this still requires *your* judgement, and your subject-matter expertise.

**The smoothing problem**

There's a specific failure mode worth watching for: homogenisation. When you ask a grounded tool to synthesise across several papers, it can tend to produce something that reads like a consensus - even when the papers actually disagree. Conflicting findings get softened into "mixed results." Fundamentally different theoretical positions get presented as complementary perspectives. The output looks balanced and considered, but the actual tensions between sources have been filed down. That is what *the middle* of a probability distribution looks like.

This is the convergence issue from last week showing up in a different form. The tool is optimised to produce coherent, readable summaries. Academic disagreement is messy and hard to summarise coherently. So it gets smoothed out. It is our task to bring it back in, or at least to ask for it, if we think that clarity on disagreement is needed to push our understanding further.

This doesn't mean grounded tools are useless for synthesis. It means you need to read the output critically. Doing so for any literature review means asking "Is this telling me these sources agree, or is it making them sound like they agree?" Where the answer matters for your work, go back to the originals on any point of claimed consensus.

**What about systematic reviews?**

Could grounded tools replace - or substantially assist - systematic or scoping reviews? That is a question that researchers are actively pursuing, and that some start-ups have staked their fortunes on. They can help with specific steps: screening titles, extracting structured data from papers, identifying themes across a set of studies. But - on their own - they can't replace the deliberate, documented search strategy that makes a review systematic. The tools don't expose their retrieval logic clearly enough and they miss papers for unpredictable reasons. Their synthesis also doesn't meet the standards of transparency that systematic reviews require.

Much of this can be improved when AI algorithms are included into more specialised tools, and these are cropping up faster than researchers can validate them. As aids within a structured workflow, they can save time. Some, such as ASReview, are based on transparent machine learning algorithms and help to cut down the long tail, so that we don't need to read huge numbers of clearly irrelevant abstracts. However, AI tools are not (yet) ready to take on the entire workflow of a systematic review - let alone to come up with good questions that are worth reviewing.

## Try this: triangulation test (5-8 min)

Pick one paper you need to read for current work (or because you are interested in it) - just something you haven't yet read in detail.

Ask a grounded tool (e.g., NotebookLM with the paper uploaded) for:

- 5 key claims the paper makes
- 3 areas of uncertainty or limitation the authors acknowledge
- 5 methodological details worth inspecting

Now spend 5 minutes with the actual paper: read the abstract, skim the figures and tables, glance at the discussion. Compare:

- What did the tool get right?
- What did it overstate or miss?
- Was there anything in the figures or tables that the tool couldn't access or interpret?

If you have time, try one more thing: ask a regular chat LLM (with the paper uploaded) the same questions about this paper. Was it as transparent as a fully grounded tool? Did it do anything better by being less restricted?

**Journal prompt**

*This time with a question I am continuously thinking about:*  Most of us have a reading list that grows faster than we can get through it. AI tools can help you cover more ground - but skimming AI summaries isn't the same as sitting with a paper and letting it reshape how you think. Where in your work does breadth matter most? Where does deep reading do something that a summary can't replace?