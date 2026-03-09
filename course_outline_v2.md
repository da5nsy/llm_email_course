# DRA GenAI Email Course - Consolidated Outline (v2)

## Course title
**Generative AI in Research: Use It Well, Use It Critically**

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
3. Grounded tools (NotebookLM-style tools, working with your own documents)
4. Writing with AI (editing, voice, cognitive ownership)
5. AI-assisted coding and data analysis (chat-to-IDE workflow, verification, forking paths)
6. Agents (coding agents as general-purpose tools, working in your context)
7. Agent workflows (bounded projects, acceptance criteria)
8. Governance, SOP, and staying current

**The "no agents" path**: Someone who does W1-6 but doesn't adopt agents has learned to use chat effectively, work with grounded tools, use AI for writing, and do AI-assisted data analysis. That's a complete, valuable toolkit. Agents (W7-8) are the advanced track.

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
**Subject:** [GAIR] Your AI baseline

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

2. Tool comparison: ask 2-3 tools the *same* question on a topic you know well. Suggested prompts (pick one, or adapt to your field):
   - "Explain X in plain language for a smart non-expert."
   - "Recommend 6 foundational readings for X and explain why each matters."
   - "Propose 3 plausible hypotheses about X and how you'd test them."

   Note: what was helpful? What was wrong? What was persuasive-but-flimsy?

**What AI should I use?**
We generally don't recommend specific models - this becomes outdated fast, and the choice depends on your preferences, budget, and language. Check the main providers (OpenAI's ChatGPT, Google's Gemini, Anthropic's Claude) and leading open-source models (Kimi, Minimax, DeepSeek, GLM, Mistral). Leaderboards like https://artificialanalysis.ai/leaderboards/models can guide exploration. Multi-model providers like https://t3.chat/ let you compare without multiple subscriptions. Most activities work without a paid subscription if you're willing to switch between providers.

**FORRT Slack:** Introduce the channel. Invite participants to share their AI autobiography or one surprising finding from the tool comparison.

**Journal:** Copy AI autobiography as first journal entry. What do you currently trust AI for? What are your red lines?

---

### Email 1B (Anchor)
**Subject:** [GAIR] What you probably noticed: confidence, drift, and context

**Purpose:** Install a correct mental model without toy simplifications.

**Core concepts:**
- LLMs predict how text would continue - word by word
  - Tokenisation, then learning patterns of associations
- Whether this is "genuine understanding" or "sophisticated pattern-matching" is an open debate (ref: Summerfield, *These Strange New Minds*) - introduced neutrally
- Fine-tuning and RLHF: models are trained by human raters to prefer certain styles of response → optimised for sounding clear and confident, not for truth. Introduces sycophancy concept (reinforced in W2B)
- Next-token prediction is context-conditioned (long text, not just a sentence); conversation drift as a consequence
- AI can generate text from a short prompt or transform existing text (summarise, critique, reformat) — transform mode tends to be more reliable

**Exercise (5-8 min): Context continuation game**
1. Take a paragraph you wrote (intro, methods, email). Delete the last 1-2 sentences.
2. Ask the model to continue for one paragraph.
3. Compare: did it match your style? Add new claims? Flatten nuance?

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
- Building on W1B's introduction of RLHF: sycophancy in practice — models default to agreement, praise, and confidence. Demo this directly.
- Training data and knowledge cut-offs shape (i.e. bias) outputs — models reflect what's in their training data, have blind spots for recent or underrepresented topics (moved from W1B; reinforces "why be critical")
- Models have improved, but critical engagement with outputs remains essential
- There are fancy names for this habit of healthy scepticism - "epistemic vigilance," the Royal Society's motto "nullius in verba" (take nobody's word for it) - but the practice is simple: check before you trust
- **Asymmetry rule**: AI is most useful where generation is costly for you and verification is cheap. It's riskiest where verification is hard or expensive.
- Search-grounded tools help with retrieval but not with judgment (deferred to W4; only briefly foreshadowed here)

**Exercise (8-10 min): Sycophancy demo → High-ROI audit**

Start here (2 min): Take one of your research ideas and prompt an AI with: "Praise this idea; assume it's correct." Then try: "Attack this idea; assume it's flawed." Compare the tone and specificity. Notice how easily it switches.

Then (5-8 min): List 5 research tasks you do often. For each, rate: how costly is it for you to generate this from scratch? How easy is it to verify the output? How bad is it if it's wrong? Identify 2 high-ROI uses for AI and 1 danger-zone task where you should be cautious.

**Further reading:**
- https://openai.com/index/why-language-models-hallucinate/

**Journal:** Which of your tasks have cheap verification? Where is verification expensive? Has the sycophancy demo changed how you read AI responses?

---

## Week 3 - Prompting, ideation, and the convergence trap

### Email 3A (Spark)
**Subject:** [GAIR] Prompt hacks are mostly theatre

**Purpose:** Prompting as specification and interaction, not magic.

**Core concepts:**
- Most "hacks" matter less than clarity of intent
- Roles/personas and few-shot examples calibrate output
- Specifying expectations helps, but broad exploration has its value - think interaction, not one-shot
- Thinking modes can help on hard tasks; they don't guarantee truth
- Different models have different strengths - ensemble of specialists (within and across)
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
**Subject:** [GAIR] Better ideas, more of the same

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

**De-convergence protocol (pick one, 3-5 min):**
- "What assumption am I making here that I should think about again?"
- "Give me five rival hypotheses that would explain the same pattern without invoking [your main mechanism]."
- "What would be an unconventional approach to testing this idea?"

**Journal:** Where did AI help you think differently? Where did it push you toward the obvious?

---

# Part 2: Working with Sources, Writing, and Data (Weeks 4-6)

## Week 4 - Grounded tools: working with your own sources

### Email 4A (Spark)
**Subject:** [GAIR] Chatbots are not search engines

**Purpose:** Introduce grounded tools and why they matter.

**Core concepts:**
- Chat LLMs ≠ search. They generate plausible text, not retrieved facts.
- Grounded tools (RAG - Retrieval Augmented Generation) retrieve from a specific corpus and cite sources
- Key distinction: tools grounded in *your* documents (NotebookLM) vs tools grounded in *published literature* (Elicit, Consensus) vs tools grounded in *web search* (Perplexity)
- Source attribution is the key feature: can you trace a claim back to a specific passage?
- In practice, you'll combine tool types - discovering papers with one, synthesising with another, checking claims with a third. Document what you used and what you verified.

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
**Subject:** [GAIR] Grounding helps retrieval, not judgment

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

**Journal:** How does grounded tool output compare to a Wikipedia entry or review paper on a topic you know? How do you judge nuance, balance, confidence?

---

## Week 5 - Writing with AI

### Email 5A (Spark)
**Subject:** [GAIR] Writing is thinking: keep cognitive ownership

**Purpose:** Use AI for clarity without outsourcing synthesis or stance.

**Core concepts:**
- Writing is a mode of thinking, not just reporting. Outsourcing the writing can mean outsourcing the thinking.
- AI for editing (clarity, structure, flow) vs AI for generating (arguments, interpretation, stance) - the distinction matters
- The two-pass approach: use AI for structural critique first, then style smoothing with constraints
- The "composite voice" problem: AI produces generic, polished prose that sounds like everyone and no one
- Reflect: what's hard for you in writing? Where do your ideas actually happen? If AI does the drafting, who does the thinking?

**Exercise (10-12 min): Two-pass writing**
1. Take a paragraph from work in progress.
2. Pass 1: Ask AI for a logic-only critique (no rewriting, just identify where logical connections are missing or weak).
3. You revise based on the critique.
4. Pass 2: Ask AI for style smoothing with constraints: "no new claims; highlight any changes that alter meaning."
5. Compare: which pass was more useful? What did the AI change that you'd want to change back?

**Journal:** Where in your writing process is AI most helpful? Where does it get in the way of your thinking?

---

### Email 5B (Anchor)
**Subject:** [GAIR] When everyone's prose sounds the same

**Purpose:** Peer review, convergence in writing, and the limits of polish.

**Core concepts:**
- AI for self-review (pre-submission stress test): acceptable and useful
- AI for reviewing others' confidential manuscripts: ethically problematic (confidentiality, intellectual laziness)
- Even individually better reviews could converge, reducing the diversity of perspective that peer review depends on
- Check your journal/conference policies - many now require disclosure of AI use in writing and reviewing
- The polish trap: AI can make anything sound smooth. But smooth isn't the same as clear, and clear isn't the same as right.

**Exercise (5-8 min): The edit audit**
1. Take a paragraph you wrote recently and ask AI to edit it for clarity.
2. Compare the original and edited versions side by side.
3. Note: what's genuinely better? What's lost (voice, hedging that was intentional, nuance)?
4. Would a reader know which version was yours?

**Journal:** How do you tell the difference between polish that helps and polish that flattens?

---

**Midpoint check-in email (after Week 5B)**

**Subject:** [GAIR] Halfway: what's changed in your practice?

- No need to catch up; each email stands alone.
- First half: mental models, chat, grounded tools, writing. Next half: hands-on data work, agents, governance.
- Reflection prompt (reply-to-email): "One habit you've started - or one temptation you've noticed - since Week 1?"
- Reminder: FORRT Slack channel for sharing experiences.
- Recommitment invitation: "If you've fallen behind, this is a good re-entry point. The next five weeks are the most hands-on."

---

## Week 6 - AI for coding and data

### Email 6A (Spark)
**Subject:** [GAIR] Let it write your code, then check everything

**Purpose:** Hands-on data analysis using the chat-to-IDE code workflow. IDE-first, with browser tools positioned for exploratory analysis.

**Core concepts:**
- Using AI to write code via chat, then running it in a local environment (RStudio, Jupyter, etc.)
- Browser tools (ChatGPT code interpreter, Claude artifacts) positioned for quick exploratory looks at data; Google Colab as backup for those without a local setup
- The copy-paste loop: describe analysis, get code, paste into IDE, hit error, paste error back, iterate
- Code that runs is not code that's right: AI-generated code can execute without errors but produce wrong results. Domain knowledge catches silent failures.
- Verification as half the job: sanity checks on sample sizes, scale direction, descriptive statistics
- Data privacy considerations when sharing data with AI tools
- Forward reference to W7 agents as solution to copy-paste friction

**Exercise (10-15 min): AI-assisted data analysis**
1. Take a dataset you're working with (or a public dataset, e.g. from GSS, Harvard Dataverse).
2. Ask a chat LLM to write code for a specific analysis.
3. Run the code in your environment (or Google Colab if no local setup).
4. Iterate: paste errors back, check output against expectations.
5. Sanity check: sample sizes, scale direction, descriptive statistics.

**Journal:** What did the AI get right that would have taken you a while? What did it get wrong that you almost missed? How did the copy-paste workflow feel?

---

### Email 6B (Anchor)
**Subject:** [GAIR] When cheap iteration becomes a risk

**Purpose:** The forking-paths problem. Pre-commitment as discipline.

**Core concepts:**
- AI lowers the cost of trying analytical alternatives - easy iteration becomes p-hacking-by-accident
- Models actively resist deliberate p-hacking requests, but the risk is undisciplined exploration by the researcher, and sycophantic framing can bypass guardrails
- Pre-commitment: decide your primary analysis before running alternatives
- AI strengthens the case for pre-registration - and can help draft one (listing decision points, simulating data, drafting code)
- Practical habit: keep a log of what you tried and why

**Exercise (5-8 min): Map your analytic choices**
1. Take an analysis you ran (or plan to run).
2. Ask an AI to list all reasonable analytic choices and decision points.
3. Evaluate which are genuinely plausible given theory and disciplinary conventions.
4. Pick one primary plan and write a one-sentence pre-commitment.

**Journal:** How many analytic choices did the AI surface that you hadn't considered? Does that change your thinking about pre-registration?

---

# Part 3: Agents (Weeks 7-8)

## Week 7 - From browser to local: introducing agents

### Email 7A (Spark)
**Subject:** [GAIR] What changes when AI works in your context

**Purpose:** Motivate agents from the browser coding friction. Demystify what agents are.

**Core concepts:**
- So far: you've been copying text into chat windows, uploading files to browser tools, pasting errors back. The AI only sees what you give it.
- Agents work differently: they see your files, execute code locally, iterate across steps without you copying anything
- "Coding agents" are misleadingly named - they're general-purpose tools that happen to be good at code. They can plan, research, organise, draft, and critique.
- Callback to W6 friction: "Remember the copy-paste loop - shuttling code and errors between chat and your editor? What if the AI could just work in your project folder?"
- Brief mention: open vs closed models, local vs cloud - agents make this practically relevant (what data leaves your machine?)

**Exercise (10-15 min): Agent meets your project**
- If you have access to an agent tool (Claude Code, Cursor, GitHub Copilot, Windsurf, etc.): point it at a project folder. Ask it to summarise what's there and identify gaps, or redo part of a W6 analysis locally.
- If not: try a free-tier option or an extended conversation where you upload multiple files and ask for a structured plan across them.
- Note: what could the agent do that the browser workflow couldn't? What felt different about not having to copy-paste?

**Journal:** What surprised you about what the agent could/couldn't do? Where did the browser-to-local shift matter most?

---

### Email 7B (Anchor)
**Subject:** [GAIR] The jagged frontier: spectacular and silently wrong

**Purpose:** Build judgment about when to trust agent output.

**Core concepts:**
- Agents make mediocre work trivially easy. Excellent work remains just as hard.
- The risk isn't that agents fail obviously - it's that they fail in ways you might not notice without domain knowledge
- Verification strategies: spot-checks, sanity checks, asking the agent to identify its own uncertainties
- The generation-verification asymmetry from Week 2 applies with even more force here

**Exercise (5-8 min): Evaluate agent output**
1. Take the output from your 7A exercise (or any agent output you've produced).
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

## Week 8 - Agents for research workflows

### Email 8A (Spark)
**Subject:** [GAIR] From ad hoc to designed: bounded agent projects

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
**Subject:** [GAIR] The grunt work was training: what agents can't replace

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

# Part 4: Big Questions (Weeks 9-10)

## Week 9 - Governance and disclosure

### Email 9A (Spark)
**Subject:** [GAIR] The policies that already govern you

**Purpose:** Make governance practical, not abstract.

**Core concepts:**
- Publisher policies: GenAI cannot be a co-author; disclosure is required; human accountability is absolute
- Documentation standards converging: tool name, version, date, what task AI performed, which sections affected
- Privacy: each tool/provider you share data with needs assessment. Open vs closed models; cloud vs local. "Free" often means value extraction.
- Policies from your institution, funder, professional body, and target journals may all apply - and may conflict
- Resource proportionality: smaller models for small tasks; no need to send everything to the most powerful (and most data-hungry) option

**Exercise (10-15 min): Policy hunt + disclosure draft**
1. Locate the AI use policies that apply to you (institution, funder, 2 target journals, professional body).
2. Note: what's required? What's ambiguous? What's silent?
3. Draft a brief AI disclosure statement suitable for your next paper or thesis chapter.

**Journal:** Where are your personal red lines now vs Week 1? What's shifted?

---

### Email 9B (Anchor)
**Subject:** [GAIR] Staying current without chasing tools

**Purpose:** Build a durable habit for updating your practice.

**Core concepts:**
- New tools appear constantly. Paradigm shifts are rarer (transformers, chat, thinking, agents). How to tell the difference: does it change what's possible, or just who provides it?
- Quarterly calibration: pick 2 benchmark tasks (one low-stakes, one high-stakes), define what "pass" looks like, re-test when something changes
- People to follow for thoughtful AI-in-research commentary (e.g., Ethan Mollick, FORRT community)
- The jagged frontier shifts: what you tested earlier in the course may be different in 6 months

**Optional pointers to macro risks (brief):**
- Deskilling / skill atrophy and resulting system failures (cf. aviation)
- Model collapse (when AI is trained on AI-generated content)
- Centralisation, commercialisation, and inequality vs narrowing gaps and growth in openness
- Fraud and slop in the literature
- AGI and existential risk narratives

**Exercise (5-8 min): Quarterly calibration ritual**
1. Choose 2 benchmark tasks relevant to your work (one where AI is already good, one where it currently struggles).
2. Define what counts as "pass" for each.
3. Put a quarterly reminder in your calendar to re-test.

**Journal:** Which tools or capabilities do you expect to change most in the next year? What would make you update your SOP?

---

## Week 10 - Your SOP

### Email 10A (Spark)
**Subject:** [GAIR] Your AI SOP: boring, reusable, real

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
**Subject:** [GAIR] Final reflection

**Purpose:** Close the loop. Revisit where you started.

**Core concepts:**
- Revisit your W1 AI autobiography - what's changed in your uses, red lines, worries?
- The capability ladder you've climbed: chat → grounded tools → writing → browser coding → agents → workflows → governance
- Your SOP is a living document - update it when tools change, when you learn something, when policies shift

**Final reflection prompt (reply-to-email):**
- "One SOP rule you'd hand to a colleague starting out with AI."

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
- [ ] Week 5A-B: Draft writing emails (writing is thinking, convergence in writing)
- [ ] Week 6A: Identify/prepare public datasets for browser coding exercise (both tracks)
- [ ] Week 7A: Write agent onboarding guide (what tools to try, free options)
- [ ] Week 7B: Write qualitative sidebar with references
- [ ] Week 9A: Compile publisher policy summaries for common social science venues
- [ ] Each week: Finalise journal questions
- [ ] Optional: Identify useful prompt/interaction resources to reference (replacing prompt starter pack)
