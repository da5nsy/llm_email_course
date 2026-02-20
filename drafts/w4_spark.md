**Subject:** [GAIR] Chatbots are not search engines

---

Week 4 of 10 - Grounded tools: working with your own sources

---

For three weeks, you've been working with chat interfaces - typing prompts, reading responses, iterating. You've learned that LLMs generate plausible continuations rather than looking things up, that they hallucinate, and that their confident tone isn't a reliability signal.

Here's the practical consequence of all that: every time you ask a chat LLM a factual question, you're asking a system that can't check whether its answer is true. It doesn't search a database. It doesn't read papers. It assembles text that fits the pattern of a good answer, whether or not a good answer exists.

This is why a whole category of tools has emerged to address the problem: **grounded tools**, sometimes called **RAG tools** (Retrieval Augmented Generation). The idea is straightforward. Instead of generating answers from training patterns alone, these tools first retrieve relevant text from a specific source, then generate a response based on what they found. The output comes with citations pointing back to the source material, so you can check where claims come from.

This doesn't make them trustworthy by default. But it's a meaningful step forward.

**Three kinds of grounding**

Not all grounded tools work the same way, and the distinction matters for how you use them.

**Grounded in your documents.** Tools like Google's **NotebookLM** let you upload your own PDFs, notes, or transcripts. The AI then answers questions based on what you uploaded, citing specific passages. This is the clearest form of grounding - you control the source material, and the tool tells you where in that material it found its answer. It's useful for synthesising across a set of papers you've already collected, pulling out themes from interview transcripts, or getting a quick overview of a document set.

**Grounded in published literature.** Tools like **Elicit** and **Consensus** search across corpora of academic papers. They find relevant studies and summarise findings with citations. This is closer to a literature search assistant - useful for discovery and structured extraction, though the coverage and quality vary by field and topic.

**Grounded in web search.** Tools like **Perplexity** (and the search modes built into ChatGPT, Gemini, and others) retrieve information from the web before generating a response. The output includes links to sources. This is the broadest form of grounding but also the noisiest - web sources vary enormously in quality, and the tool's selection of what to cite isn't always transparent.

**When to use which**

This depends on what you're trying to do. If you have a specific set of documents and need to work with them - synthesise, compare, extract - document-grounded tools like NotebookLM are the right starting point. If you're looking for papers you don't have yet, literature-grounded tools like Elicit can help with discovery. And if you need quick answers about recent events, people, or topics outside the academic literature, web-grounded search tools fill that gap.

In practice, you'll probably find yourself using more than one type. Discovering papers with Elicit, then uploading them to NotebookLM for detailed synthesis, then checking a specific claim with a web search. The tools complement each other when used deliberately.

**What grounding actually gives you**

The key feature of grounded tools is **source attribution**. When a grounded tool tells you something, you can (in principle) trace the claim back to a specific passage in a specific document. This is a substantial improvement over chat, where claims float free of any source.

In practice, the tracing isn't perfect. Tools sometimes cite a paper but misrepresent what it says. They can pull a sentence from a discussion section and present it as a finding. They may cite the right paper for the wrong claim. But the ability to check - to click through and see what the source actually says - changes your verification workflow. Instead of asking "is this plausible?" you can ask "does this match what the paper says?" The second question is much easier to answer.

**What grounding doesn't give you**

Grounded tools are better at retrieval. They're not better at judgment.

They can find relevant passages across a stack of papers. They can't tell you which study was well-designed and which had fatal methodological flaws. They can extract what authors claimed, but they can't weigh the evidence the way a researcher reading carefully would. And they can still miss things - papers in your stack that are relevant but don't use the keywords the tool is looking for, or arguments that span multiple sections and don't reduce to a quotable passage.

We'll dig into these limits more on Thursday. For now, the point is that grounded tools address one of the biggest problems with chat (no source attribution) while introducing a new risk: the appearance of rigour where you still need your own judgment.

**These tools change fast**

The tools I've mentioned are current at the time of writing, but this space moves fast. NotebookLM, Elicit, and Consensus are good starting points for getting a feel for how grounded tools work. By the time you read this, there may be newer options worth trying. The underlying concept - retrieve first, then generate, and show your sources - is what matters. Any tool built on that principle is worth exploring. [NEEDS CHECK: verify these tools are still available and free/freemium at time of sending]

## Try this: grounded synthesis test (10-15 min)

Choose 5-10 papers relevant to a current project. If you don't have a set ready, pick a topic and grab a few from Google Scholar - they don't need to be ones you've read carefully.

Upload them to **NotebookLM** (free with a Google account) or another grounded tool that lets you upload your own documents.

Then ask:

1. "What are the main areas of agreement across these papers?"
2. "Where do they disagree?"
3. "What methodological limitations are shared across these studies?"

For each answer, check:

- Does the tool cite specific papers for each claim?
- Click through (or check) at least 2-3 citations. Does the paper actually say what the tool claims?
- Did the synthesis surface anything you hadn't noticed in your own reading?
- Did it miss anything important that you know is in the papers?

If you don't have time for the full exercise, even uploading 2-3 papers and asking one question will give you a feel for how this works.

**Journal prompt**

What did the grounded tool surface that you hadn't noticed? What did it miss or flatten? How does this compare to the experience of asking a chat LLM about the same topic?
