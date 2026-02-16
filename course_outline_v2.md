# DRA GenAI Email Course - Consolidated Outline (v2)

## Course title
**Getting Started with Generative AI in Research** (working title - TBD)

## Audience
Social scientists interested in making their research better and more efficient. Not specifically PhD students - no supervision/training focus. Assumes quantitative orientation; qualitative data analysis is optional/sidebar only.

## Format
- 10 weeks, 2 emails per week
- **Email A (Monday, Spark)**: 10-15 minutes, one concrete exercise
- **Email B (Thursday, Anchor)**: 5-10 minutes, debrief + critical lens + durable takeaway
- Midpoint check-in email after Week 5
- Sign up at any time, fully asynchronous
- Feedback by email; peer exchange on FORRT Slack channel (encouraged at start, midpoint, end)

## Tone
Informal, inviting independence. Not prescriptive. Acknowledges tensions honestly rather than resolving them neatly.

## Capability ladder (course backbone)
1. What LLMs are (mental model)
2. Chat interfaces (interactive use, prompting, critical evaluation)
3. Grounded models (NotebookLM-style tools, working with your own documents)
4. Agents (coding agents as general-purpose tools, research workflow automation)
5. Applied challenges woven throughout, intensifying in final weeks

## Learning objectives
Participants will learn to:

1. **Interact effectively with GenAI (co-intelligence)**
   - Capability-aware planning from the start
   - Iterative exploration (multi-turn collaboration)
   - Prompt design as specification (constraints, roles, examples)

2. **Interact critically (epistemic vigilance)**
   - Understand hallucination, sycophancy, bias, and confidence miscalibration
   - Know where humans must retain judgment and control
   - Practice transparency and responsible disclosure

3. **Understand GenAI beyond simplistic "next-token only" claims**
   - Grounded/RAG tools: what they help with, what they don't
   - Thinking / extended reasoning modes
   - Agentic workflows as *intensifiers* of both benefits and risks

## Course artifact: Reflective journal
Replaces the prompt library concept. A simple template (Google Doc) with:
- 2-3 guided questions per week (specific to that week's content)
- A running "jagged frontier" section: what AI handles well / what still needs me
- Feeds directly into the Week 10 SOP draft
- Participants can take notes elsewhere if they prefer; the journal provides structure without pressure

---

# Part 1: Foundations & Chat (Weeks 1-3)

## Week 1 - What LLMs are (and aren't)

### Email 1A (Spark)
**Subject:** [GAIR] What do you trust AI for (and why)?

**Purpose:** Establish a personal baseline. Begin capability-aware planning.

**Core concepts:**
- LLMs have hugely accelerated some areas of work
- LLMs generate plausible continuations, not truth
- Confidence is a style feature, not a reliability signal
- Different models behave differently; treat them as distinct collaborators

**Exercise (10-15 min): AI autobiography + tool comparison**

1. AI autobiography (6 bullet points):
   - Current uses
   - Perceived benefits
   - Pitfalls experienced
   - Biggest worry
   - Current red lines / tasks you refuse to outsource
   - Goals for this course

2. Tool comparison: ask 2-3 tools the *same* question on a topic you know well. Suggested prompts (pick two):
   - "Explain X in plain language for a smart non-expert."
   - "Recommend 6 foundational readings for X and explain why each matters."
   - "Propose 3 plausible hypotheses about X and how you'd test them."

   Note: what was helpful? What was wrong? What was persuasive-but-flimsy?

**What AI should I use?**
We generally don't recommend specific models - this becomes outdated fast, and the choice depends on your preferences, budget, and language. Check the main providers (OpenAI's ChatGPT, Google's Gemini, Anthropic's Claude) and leading open-source models (Kimi, Minimax, DeepSeek, GLM, Mistral). Leaderboards like https://artificialanalysis.ai/leaderboards/models can guide exploration. Multi-model providers like https://t3.chat/ let you compare without multiple subscriptions. Most activities work without a paid subscription if you're willing to switch between providers.

**FORRT Slack:** Introduce the channel. Invite participants to share their AI autobiography or one surprising finding from the tool comparison.

**Journal:** What do you currently trust AI for? What are your red lines?

---

### Email 1B (Anchor)
**Subject:** [GAIR] What you probably noticed: confidence, drift, and context

**Purpose:** Install a correct mental model without toy simplifications.

**Core concepts:**
- LLMs predict how text would continue - word by word
  - Tokenisation, then learning patterns of associations
- "Stochastic Parrot" vs "emergent reasoning" debate (introduced neutrally)
- Next-token prediction is context-conditioned (long text, not just a sentence)
- Training data and knowledge cut-offs shape (i.e. bias) outputs
- AI can generate text from a short prompt or transform information (e.g. from PDFs)
- Brief mention: open vs closed models, local vs cloud - we'll return to this in Week 8 when we talk about privacy and governance

**Exercise (5-8 min): Context continuation game**
1. Take a paragraph you wrote (intro, methods, email). Delete the next 1-2 sentences.
2. Ask the model to continue without adding new factual claims.
3. Compare: where did it match style but flatten nuance or sneak in new claims?

**Journal:** Revisit your tool comparison from 1A. Now that you know more about how LLMs work, does anything make more sense?

---

## Week 2 - Confident errors: hallucination, sycophancy, epistemic vigilance

### Email 2A (Spark)
**Subject:** [GAIR] The citation your AI just invented

**Purpose:** Make hallucination tangible - both citation fabrication and factual confabulation. Show that self-verification sometimes helps but isn't reliable.

**Core concepts:**
- Models produce citation-shaped text without retrieval - unique combinations of many words (like full references) are particularly failure-prone
- This extends beyond citations: AI also fabricates plausible-sounding facts, statistics, and historical claims
- This isn't a bug - it's a predictable consequence of the architecture (from Week 1: plausible continuation, not truth)
- Models can sometimes catch their own errors when asked to verify - but not always, and not reliably

**Exercise (10-15 min): Hallucination hunt**

Main track: Ask a chat LLM for 6 citations supporting a niche claim you know well. Verify existence and whether each actually supports the claim. Label each: real / fabricated / Frankenstein (real author + journal, fake title) / misattributed / outdated. Then: paste the citations back and ask the model to check which ones are real. How accurate is its self-assessment?

If you already know about citation hallucination: Try asking about factual claims at the edge of your expertise - a topic you know something about but aren't certain of the details. Ask the AI to make specific empirical claims (statistics, dates, study findings). How hard is it to tell what's real when you're not already an expert?

**Journal:** How confident did the AI sound when giving you wrong information? Did self-verification help? How does this change your trust calibration?

---

### Email 2B (Anchor)
**Subject:** [GAIR] Why it tells you what you want to hear

**Purpose:** Explain sycophancy. Introduce the generation-verification asymmetry as a practical decision rule.

**Core concepts:**
- RLHF (reinforcement learning from human feedback) pushes toward pleasing, agreeable responses - in one-off interactions, this can mean uncritical praise and confident fabrication
- Models have improved, but critical engagement with outputs remains essential
- There are fancy names for this habit of healthy scepticism - "epistemic vigilance," the Royal Society's motto "nullius in verba" (take nobody's word for it) - but the practice is simple: check before you trust
- **Asymmetry rule** (moved from 1B): AI is most useful where generation is costly for you and verification is cheap. It's riskiest where verification is hard or expensive.
- Search-grounded tools help with retrieval but not with judgment

**Exercise (8-10 min): Sycophancy demo → High-ROI audit**

Start here (2 min): Take one of your research ideas and prompt an AI with: "Praise this idea; assume it's correct." Then try: "Attack this idea; assume it's flawed." Compare the tone and specificity. Notice how easily it switches.

Then (5-8 min): List 5 research tasks you do often. For each, rate: how costly is it for you to generate this from scratch? How easy is it to verify the output? How bad is it if it's wrong? Identify 2 high-ROI uses for AI and 1 danger-zone task where you should be cautious.

**Further reading:**
- https://openai.com/index/why-language-models-hallucinate/

**Journal:** Which of your tasks have cheap verification? Where is verification expensive? Has the sycophancy demo changed how you read AI responses?

---

## Week 3 - Prompting, ideation, and the convergence trap

### Email 3A (Spark)
**Subject:** [GAIR] 3A. Prompt hacks are mostly theatre

**Purpose:** Prompting as specification and interaction, not magic.

**Core concepts:**
- Most "hacks" matter less than clarity of intent
- Roles/personas and few-shot examples calibrate output
- Specifying expectations helps, but broad exploration has its value - think interaction, not one-shot
- Thinking modes can help on hard tasks; they don't guarantee truth
- Different models have different strengths - ensemble of experts (within and across)
- Many technical prompting tips no longer necessary for top models (they're trained to understand intent), but they can help users clarify their own intent

**Exercise (10-12 min): Iteration ladder**
Pick a real research task and run 4 prompts:
1. Vague
2. Constrained (clear task + output format)
3. Role-based (add persona)
4. Few-shot (add examples of desired output)

Compare results. Where did specificity help most?

**Journal:** Which 2-3 prompting moves actually changed your results?

---

### Email 3B (Anchor)
**Subject:** [GAIR] 3B. Better ideas, more of the same: the convergence problem

**Purpose:** Apply prompting to ideation; introduce convergence as structural risk.

**Core concepts:**
- AI as a brainstorming/sparring partner - useful for critique, stress-testing, cross-disciplinary connections
- AI can raise individual idea quality but increase convergence across ideas (Wharton study; *Nature* study of 41M papers showing AI-assisted research clusters around popular topics, covers less intellectual territory)
- Socratic prompting: ask AI to challenge your thinking, not confirm it
- Adversarial prompting: task AI with generating counter-hypotheses, identifying confounding variables

**Exercise (10 min): Reviewer #2 stress test**
1. Paste your research question, abstract, or brief project description.
2. Ask for fatal flaws + fixable weaknesses (use a "skeptical senior reviewer" persona).
3. Write a human rebuttal for the top 3 critiques.

**De-convergence protocol (pick one, 5 min):**
- Ask for boundary cases where your hypothesis fails
- Ask for rival hypotheses explaining the same pattern
- Ask for reverse argumentation (strongest case against your position)

**Journal:** Where did AI help you think differently? Where did it push you toward the obvious?

---

# Part 2: Grounded Tools & Synthesis (Weeks 4-5)

## Week 4 - Grounded tools: working with your own sources

### Email 4A (Spark)
**Subject:** [GAIR] 4A. Chatbots are not search engines

**Purpose:** Introduce grounded tools and why they matter.

**Core concepts:**
- Chat LLMs ≠ search. They generate plausible text, not retrieved facts.
- Grounded tools (RAG - Retrieval Augmented Generation) retrieve from a specific corpus and cite sources
- Key distinction: tools grounded in *your* documents (NotebookLM) vs tools grounded in *published literature* (Elicit, Consensus) vs tools grounded in *web search* (Perplexity)
- Source attribution is the key feature: can you trace a claim back to a specific passage?

**Recommended tools to try:**
- **NotebookLM** (Google, free) - upload your own PDFs, get source-attributed Q&A. Clearest example of document grounding.
- **Elicit** - grounded in academic paper corpus, good for literature discovery and structured extraction.
- **Consensus** - searches across published research, summarises with citations.
- The landscape evolves quickly; these are starting points, not endorsements.

**Exercise (10-15 min): Grounded synthesis test**
1. Choose 5-10 papers relevant to a current project.
2. Upload them to NotebookLM (or equivalent grounded tool).
3. Ask: "What are the main areas of agreement across these papers? Where do they disagree?"
4. Ask: "What methodological limitations are shared across these studies?"
5. Check: does the tool cite specific papers for each claim? Are the citations accurate?

**Journal:** What did the grounded tool surface that you hadn't noticed? What did it miss or flatten?

---

### Email 4B (Anchor)
**Subject:** [GAIR] 4B. Grounding helps retrieval - not judgment

**Purpose:** Explain RAG and its limits. Teach triangulation.

**Core concepts:**
- RAG/search tools are better at traceability than raw chat
- Still weak at weighting evidence, identifying subtle caveats, and recognising when sources disagree substantively
- Homogenisation risk: grounded tools can still smooth out conflicting academic voices into bland consensus
- For systematic or scoping reviews, grounded tools are aids, not replacements - stricter workflows needed

**Exercise (5-8 min): Triangulation test**
1. Pick one paper you need to read for current work.
2. Ask a grounded tool for: 5 claims; 3 uncertainties; 5 methods details to inspect.
3. Compare with: abstract + skim figures/tables + your own judgment.
4. Note: what did the tool miss? What did it overstate?

**Further exploration:**
- Compare the same question across: raw chat LLM, grounded tool, and traditional database search (Google Scholar, PubMed). What sources appear? What's the overlap?

**Journal:** How does grounded tool output compare to a Wikipedia entry or review paper on a topic you know? How do you judge nuance, balance, confidence?

---

## Week 5 - Literature workflows and the transition to agents

### Email 5A (Spark)
**Subject:** [GAIR] 5A. Building a literature workflow that actually holds up

**Purpose:** Practical literature work combining human retrieval with AI synthesis.

**Core concepts:**
- The human finds and validates sources; AI helps with comparison, extraction, and gap identification
- Documentation matters: which tools used, what queries, what was verified
- AI is interdisciplinary - boon (cross-field connections) and curse (flattening disciplinary nuance)

**Exercise (10-15 min): Literature comparison**
1. Take a specific research question you're working on.
2. Search for it using: (a) traditional database search, (b) a chat LLM, (c) a grounded literature tool (Elicit/Consensus).
3. Compare: coverage, accuracy, novelty of sources found, quality of synthesis.
4. Draft a brief note: which approach found what, and what workflow would you use going forward?

**Journal:** What's your emerging literature workflow? What role does each tool type play?

---

### Email 5B (Anchor)
**Subject:** [GAIR] 5B. From copying and pasting to working in context

**Purpose:** Motivate the shift from chat to agents. Bridge to Part 3.

**Core concepts:**
- So far: you've been copying text into chat windows and grounded tools. The AI only sees what you paste.
- Agents work differently: they can see your files, operate across documents, execute multi-step tasks, and iterate on their own work.
- "Coding agents" are misleadingly named - they're general-purpose tools that happen to be good at code. They can plan, research, organise, draft, and critique.
- The shift: from "I paste, it responds" to "it works in my context."
- This intensifies both benefits AND risks.

**Exercise (10 min): Your first agent interaction**
- If you have access to an agent tool (Claude Code, Cursor, GitHub Copilot, etc.): point it at a project folder containing some notes, a draft, and/or a few papers. Ask it to help you plan next steps for the project, or to summarise what's in the folder and identify gaps.
- If not: try a free-tier agent or extended conversation where you upload multiple documents and ask for a structured plan across them.
- Note: what could the agent do that chat couldn't? What felt different?

**Journal:** What surprised you about what the agent could/couldn't do?

---

**Midpoint check-in email (after Week 5B)**

**Subject:** [GAIR] Halfway: what's changed in your practice?

- No need to catch up; each email stands alone.
- Next half focuses on agents, data analysis, writing, and governance.
- Reflection prompt (reply-to-email): "One habit you've started - or one temptation you've noticed - since Week 1?"
- Reminder: FORRT Slack channel for sharing experiences.
- Recommitment invitation: "If you've fallen behind, this is a good re-entry point. The next five weeks are the most hands-on."

---

# Part 3: Agents (Weeks 6-8)

## Week 6 - Agents are general-purpose tools

### Email 6A (Spark)
**Subject:** [GAIR] 6A. Your new research assistant works locally

**Purpose:** Demystify agents. Show breadth of capability beyond coding.

**Core concepts:**
- What agents actually are: systems that operate with your project in context, can read/modify files, execute code, and iterate across multiple steps
- Key difference from chat: stateful, multi-step, working with your actual files
- The jagged frontier sharpened: agents are spectacular at some tasks and silently wrong at others, and the boundary is unpredictable. Testing per task is essential.
- Examples of non-coding agent tasks: organising literature notes, drafting structured summaries from multiple documents, comparing datasets, generating project plans

**Exercise (10-15 min): Bounded agent task**
Choose one:
- **Planning/organising:** Point an agent at a set of project files and ask it to create a structured summary of where things stand + what's missing.
- **Text analysis:** Give an agent ~20 open-ended survey responses or interview transcripts (from a public source or your own non-sensitive data - e.g. the [Reading the Riots transcripts](https://reshare.ukdataservice.ac.uk/853792/)) and ask it to extract and categorise themes. Compare to your own reading of the responses.
- **Literature extraction:** Give an agent 3-5 PDFs and ask it to produce a comparison table (claims, methods, limitations, gaps).

**Journal:** What surprised you about what the agent could/couldn't do? Where was the jagged frontier?

---

### Email 6B (Anchor)
**Subject:** [GAIR] 6B. The jagged frontier: spectacular and silently wrong

**Purpose:** Build judgment about when to trust agent output.

**Core concepts:**
- Agents make mediocre work trivially easy. Excellent work remains just as hard.
- The risk isn't that agents fail obviously - it's that they fail in ways you might not notice without domain knowledge.
- Verification strategies: spot-checks, sanity checks, asking the agent to identify its own uncertainties.
- The generation-verification asymmetry from Week 2 applies with even more force here.

**Exercise (5-8 min): Evaluate agent output**
1. Take the output from your 6A exercise.
2. Identify: 2 things the agent got right that saved you time; 1 thing it got wrong or oversimplified.
3. How would you have caught the error if you weren't already an expert on this?

**Sidebar (optional): Qualitative data analysis with agents**
- AI can perform keyword detection and surface-level categorisation
- Struggles with latent/interpretive coding - generates more literal/descriptive codes than a human researcher would
- Epistemological tensions with reflexive qualitative traditions are real and unresolved
- If interested: Morgan (2023) on AI as assistant in early phases of interpretive process; open letter debates on AI and reflexive thematic analysis
- Best current use: secondary reliability check, not primary coder

**Journal:** How would you explain to a colleague what the agent did and what you did?

---

## Week 7 - Agents for data analysis

### Email 7A (Spark)
**Subject:** [GAIR] 7A. Let it run your analysis - then check everything

**Purpose:** Hands-on data analysis with agents. Two tracks.

**Core concepts:**
- Coding agents for quant work: data cleaning, visualisation, exploratory analysis, statistical modelling
- The critical caveat: code may run without errors but produce incorrect results
- You need domain knowledge to validate outputs - this is augmentation, not automation
- Relevance of test-driven thinking: specify expected outputs before running

**Exercise (10-15 min): Two tracks**

*Quant track:*
1. Take a dataset you're working with (or a public dataset, e.g. from GSS, ANES, Pew).
2. Give an agent a specific analysis question (e.g., "Explore the relationship between X and Y, controlling for Z").
3. Have it write and run the analysis.
4. Check: Does the code do what you asked? Are the results plausible? Run a "broken legs" sanity check (impossible values, coding inversions, missingness patterns).

*Text analysis track:*
1. Take a set of open-ended responses or interview transcripts (from a public source or your own non-sensitive data, ~20-50 responses). A good freely available option: the [Reading the Riots transcripts](https://reshare.ukdataservice.ac.uk/853792/) (Guardian/LSE study of the 2011 English riots - 224 redacted interview transcripts).
2. Ask an agent to: (a) summarise main themes, (b) create a simple coding scheme, (c) apply it to the responses.
3. Read 10 responses yourself first. Compare: what did the agent catch? What did it flatten or miss? Where did it impose categories that don't fit?

**Journal:** What did the agent get right that would have taken you hours? What did it get wrong that you almost missed?

---

### Email 7B (Anchor)
**Subject:** [GAIR] 7B. When cheap iteration becomes a confound

**Purpose:** The forking-paths problem. Pre-commitment as discipline.

**Core concepts:**
- AI lowers the cost of trying analytical alternatives → explosion of forking paths
- This isn't inherently bad, but without discipline it becomes p-hacking-by-accident
- Pre-commitment: decide your primary analysis before running alternatives
- "Broken legs" checks: cheap sanity checks that catch obvious data problems before substantive analysis
- Synthetic/simulated data: useful for testing pipelines, dangerous for inference

**Exercise (8-10 min):**
1. Take an analysis you ran (or plan to run).
2. Ask an agent to list all reasonable analytic choices and decision points.
3. Pick one primary plan and write a one-sentence pre-commitment: "Primary analysis will be [X] unless [predefined condition Y occurs], in which case we will [Z]."

**Further exploration:**
- Multimodal extraction: screenshot a table/chart from a PDF, ask a model to transcribe to CSV, spot-check 5 random cells. High-ROI where verification is cheap.

**Journal:** How many analytic choices did the agent surface that you hadn't considered? How does that change your thinking about pre-registration?

---

## Week 8 - Agents for research workflows

### Email 8A (Spark)
**Subject:** [GAIR] 8A. From ad hoc to designed: bounded agent projects

**Purpose:** Design and run a structured agent task with acceptance criteria.

**Core concepts:**
- Moving from "let me try this" to "here's a specified task with clear inputs, outputs, and checkpoints"
- Human-in-the-loop specs: inputs, outputs, checkpoints, acceptance criteria, failure modes
- Bounded agents are more reliable than open-ended ones

**Exercise (10-15 min): Design and run one bounded agent project**

Choose one:
- **Literature extraction table:** Inputs: 3-5 PDFs. Output: table with columns for claim, evidence location, methods note, limitation, your confidence. Acceptance criteria: every claim must have a page/section pointer or be marked "needs verification."
- **Methodology critique:** Inputs: your methods section or study design. Output: structured critique identifying assumptions, threats to validity, and suggestions. Acceptance criteria: identifies at least 2 issues you agree with and explains why.
- **Materials generation:** Inputs: study design parameters. Output: draft materials (e.g., vignettes for stimulus sampling, survey items, interview protocol). Acceptance criteria: materials match specified constraints; nothing fabricated.

**Journal:** What acceptance criteria did you set? Did the agent meet them? What would you change?

---

### Email 8B (Anchor)
**Subject:** [GAIR] 8B. The grunt work was training: what agents can't replace

**Purpose:** The supervision-of-agents problem. What human skills remain essential.

**Core concepts:**
- The "grunt work was training" paradox (Garimella): data cleaning and basic coding used to build researcher skill. When agents do this in minutes, what replaces that learning?
- Value shifts to: the questions you ask, the data you can uniquely access, domain judgment, ethical reasoning
- Agent supervision is a new skill: specifying tasks clearly, evaluating output critically, knowing when to intervene
- The jagged frontier is personal and evolves: what you can safely delegate depends on what you already know

**Exercise (5-8 min):**
1. List 10 research tasks you do regularly.
2. Classify each: human-only / AI-supported (with checks) / AI-outsourced.
3. For each AI-supported task: write one cheap verification check.
4. Circle any task where you'd lose important learning by outsourcing it.

**Journal:** Which tasks are you tempted to outsource but probably shouldn't? Why?

---

# Part 4: The Big Questions (Weeks 9-10)

## Week 9 - Writing, voice, and governance

### Email 9A (Spark)
**Subject:** [GAIR] 9A. Writing is thinking: keep cognitive ownership

**Purpose:** Use AI for clarity without outsourcing synthesis or stance.

**Core concepts:**
- Writing is a mode of thinking, not just reporting. Outsourcing the writing can mean outsourcing the thinking.
- The "composite voice" problem: AI produces generic, polished prose that sounds like everyone and no one
- AI for editing (clarity, structure, flow) vs AI for generating (arguments, interpretation, stance)
- Reflect: What's hard for you in writing? Where do your ideas happen? What's your value-add?

**Exercise (10-12 min): Two-pass writing**
1. Take a paragraph from work in progress.
2. Pass 1: Ask AI for a logic-only critique (no rewriting, just identify where logical connections are missing or weak).
3. You revise based on the critique.
4. Pass 2: Ask AI for style smoothing with constraints: "no new claims; highlight any changes that alter meaning."
5. Compare: which pass was more useful?

**Peer review boundaries (brief):**
- AI for self-review (pre-submission stress test): acceptable and useful
- AI for reviewing others' confidential manuscripts: ethically problematic (confidentiality, intellectual laziness)
- Even if AI makes each review better individually, it could make reviews converge - reducing the diversity of perspective that peer review depends on
- Check your journal/conference policies

**Journal:** Where in your writing process is AI most helpful? Where does it get in the way of your thinking?

---

### Email 9B (Anchor)
**Subject:** [GAIR] 9B. The policies that already govern you

**Purpose:** Make governance practical, not abstract.

**Core concepts:**
- Publisher policies: GenAI cannot be a co-author; disclosure is required; human accountability is absolute
- Documentation standards converging: tool name, version, date, what task AI performed, which sections affected
- Privacy: each tool/provider you share data with needs assessment. Cloud vs local. "Free" often means value extraction.
- Policies from your institution, funder, professional body, and target journals may all apply - and may conflict
- Resource proportionality: smaller models for small tasks; no need to send everything to the most powerful (and most data-hungry) option

**Exercise (10-15 min): Policy hunt + disclosure draft**
1. Locate the AI use policies that apply to you (institution, funder, 2 target journals, professional body).
2. Note: what's required? What's ambiguous? What's silent?
3. Draft a brief AI disclosure statement suitable for your next paper or thesis chapter.

**Journal:** Where are your personal red lines now vs Week 1? What's shifted?

---

## Week 10 - Your SOP and staying current

### Email 10A (Spark)
**Subject:** [GAIR] 10A. Your AI SOP: boring, reusable, real

**Purpose:** Convert the course into a document you can use and share.

**Exercise (15-20 min): Draft your SOP**
Draw on your 9 weeks of journal entries. The SOP should include:

1. **Green zone** (default allowed): tasks where you routinely use AI, with brief rationale
2. **Amber zone** (allowed with checks): for each, specify the check and what "save a receipt" looks like
3. **Red zone** (never): clear lines with short rationales
4. **Data handling rules**: what goes to cloud tools, what stays local, what never touches AI
5. **Analysis integrity**: your pre-commitment norm, your broken-legs checklist
6. **Peer review boundary**: what you'll use AI for in reviewing your own vs others' work
7. **Disclosure defaults**: your standard disclosure statement

**FORRT Slack:** Share one SOP rule you'd recommend to a colleague.

**Journal:** What's in your SOP that you wouldn't have predicted in Week 1?

---

### Email 10B (Anchor)
**Subject:** [GAIR] 10B. Staying current without chasing tools

**Purpose:** Build a durable habit for updating your practice.

**Core concepts:**
- New tools appear constantly. Paradigm shifts are rarer (transformers, chat, thinking, agents). How to tell the difference: does it change what's possible, or just who provides it?
- Quarterly calibration: pick 2 benchmark tasks (one low-stakes, one high-stakes), define what "pass" looks like, re-test when something changes
- People to follow for thoughtful AI-in-research commentary (e.g., Ethan Mollick, FORRT community)
- The jagged frontier shifts: what you tested in Week 6 may be different in 6 months

**Exercise (5-8 min): Quarterly calibration ritual**
1. Choose 2 benchmark tasks relevant to your work (one where AI is already good, one where it currently struggles).
2. Define what counts as "pass" for each.
3. Put a quarterly reminder in your calendar to re-test.

**Optional further exploration (macro risks, brief pointers):**
- Deskilling / skill atrophy and resulting system failures (cf. aviation)
- Model collapse (when AI is trained on AI-generated content)
- Centralisation, commercialisation, and inequality vs narrowing gaps and growth in openness
- Fraud and slop in the literature
- AGI and existential risk narratives

**Final reflection prompt (reply-to-email):**
- "What's one SOP rule you'd hand to a colleague starting out with AI?"

**FORRT Slack:** Share your calibration benchmarks or your biggest takeaway from the course.

---

# Infrastructure TODO

- [ ] Set up FORRT Slack channel
- [ ] Create reflective journal template (Google Doc)
- [ ] Set up email delivery system (platform TBD)
- [ ] Create landing page / sign-up mechanism
- [ ] Write welcome email (with journal template link, Slack invite, what to expect)
- [ ] Identify/create public datasets for exercises (GSS, ANES, Pew, etc.)
- [ ] Build sources/references list for each week (see sources.md)
- [ ] Decide on [GAIR] branding / course title
- [ ] Draft each email in full (current outline = structural skeleton only)

# Content TODO

- [ ] Week 1A: Write "What AI should I use?" section with current tool landscape
- [ ] Week 4A: Finalise grounded tools recommendations (NotebookLM + alternatives)
- [ ] Week 5B: Write agent onboarding guide (what tools to try, free options)
- [ ] Week 6B: Write qualitative sidebar with references
- [ ] Week 7A: Identify/prepare public datasets for both tracks
- [ ] Week 9B: Compile publisher policy summaries for common social science venues
- [ ] Each week: Finalise journal questions
- [ ] Optional: Identify useful prompt/interaction resources to reference (replacing prompt starter pack)
