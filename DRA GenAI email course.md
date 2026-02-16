# **Gemini report**

# **The Augmented Academic: A Curricular Framework for Integrating Generative AI into Graduate Research Training**

## **1\. Executive Summary: The Pedagogical Pivot**

The integration of Generative Artificial Intelligence (GenAI) into the academic research ecosystem represents a paradigm shift comparable to the introduction of the internet or the personal computer. However, unlike previous technological disruptions which primarily accelerated information retrieval or computation, GenAI fundamentally alters the cognitive processes of synthesis, ideation, and analysis itself. The current landscape of AI training in higher education is frequently dominated by a "tool-centric" approach, focusing on specific applications that are often ephemeral or quickly outdated. This report argues that such an approach is insufficient for the long-term development of graduate students and early-career researchers. Instead, we propose a rigorous, 10-week curriculum titled **"The Augmented Academic,"** designed to cultivate enduring *AI literacy*, *cognitive calibration*, and *epistemic vigilance*.

This report serves as the comprehensive design document for this course. It eschews the "tips and tricks" model in favor of a "First Principles" approach, grounding every module in the emerging literature on Human-AI Collaboration (HAIC), cognitive psychology, and information science. The curriculum is structured around the **Centaur and Cyborg** frameworks 1, teaching researchers to fluidly navigate the "Jagged Frontier" of AI capability.2 It addresses critical risks such as **cognitive offloading** 3 and **model collapse** 5, ensuring that the adoption of AI enhances rather than erodes the intellectual autonomy of the researcher.

The proposed delivery mechanism—a 10-week email course with "Micro-Challenges"—is designed to fit the fragmented schedules of graduate students while enforcing a cadence of "spaced repetition" and active learning. The following sections detail the theoretical underpinnings, the week-by-week curricular content, and the ethical frameworks necessary to navigate this new epoch of research.

## ---

**2\. Theoretical Framework: Beyond Tool Proficiency**

### **2.1 The Crisis of "Magic Button" Epistemology**

The prevailing danger in current AI adoption is the "black box" phenomenon, where researchers treat LLMs as oracles of truth rather than probabilistic engines. This leads to what might be termed "Magic Button Epistemology"—the belief that a single prompt can replace the iterative struggle of inquiry. To counter this, the curriculum is built on the premise that **technical demystification is a prerequisite for ethical application**. One cannot effectively navigate the risks of hallucination 7 or bias 9 without understanding the underlying mechanisms of tokenization and next-token prediction.10

By stripping away the anthropomorphic veneer of the "chatbot," we reveal the tool as a **stochastic reasoning engine**.12 This shift in mental model is crucial. When a student understands that an LLM generates citations based on the statistical probability of tokens appearing together, rather than retrieving them from a database, the phenomenon of "hallucination" transforms from a confusing bug into a predictable feature of the architecture.13 This fundamental technical literacy forms the bedrock of the first three weeks of the course.

### **2.2 Models of Collaboration: Centaurs and Cyborgs**

The literature on human-AI interaction suggests that successful integration does not look like "automation" (where the human steps away) but rather "augmentation" (where the human steps in). The course utilizes the taxonomy proposed in recent studies by the Boston Consulting Group and academic partners, which distinguishes between two dominant modes of high-performance use:

| Mode | Definition | Cognitive Mechanism | Best Use Case | Risk Profile |
| :---- | :---- | :---- | :---- | :---- |
| **The Centaur** | A strategic division of labor where human and AI tasks are clearly compartmentalized. | **Delegation.** The user switches between "human mode" and "AI mode" based on the task type. | Data cleaning, formatting citations, summarizing distinct documents. | **Low.** Clear hand-offs allow for distinct quality control checks.1 |
| **The Cyborg** | A deep integration where human and AI efforts are intertwined at the granular level. | **Flow Integration.** The user and AI co-create in real-time, finishing each other's sentences or iterating on code line-by-line. | Ideation, drafting prose, exploratory coding. | **High.** Risk of "falling asleep at the wheel" or losing the "human voice".1 |

Table 1: Comparative Analysis of Human-AI Collaboration Models 1

The curriculum is designed to train students in *both* modalities, but crucially, to know *when* to deploy each. The "Jagged Frontier" concept 2 illustrates that AI capabilities are not uniform; an LLM might ace a complex coding challenge (Cyborg territory) but fail a simple arithmetic problem (Centaur territory where the human should take over). Mapping this frontier within one's specific discipline is a core learning objective.

### **2.3 The Risk of Cognitive Offloading and Automation Bias**

A significant portion of the curriculum is dedicated to the "Shadow Side" of AI adoption: the atrophy of critical skills. Research indicates a negative correlation between frequent, uncritical AI usage and independent critical thinking abilities.3 This phenomenon, known as **cognitive offloading**, occurs when users delegate not just the *process* (e.g., typing) but the *cognition* (e.g., structuring the argument) to the tool.4

The danger is further compounded by **automation bias**, where users place undue trust in algorithmic outputs, often ignoring contradictory information they would otherwise notice.17 In the context of research, this can lead to the acceptance of "plausible but false" methodologies or the "flattening" of nuanced qualitative data into generic themes.18 The course addresses this by introducing "Unplugged" activities 19 and "Adversarial Prompting" exercises 21 that force the student to re-engage their critical faculties and "check the work" of the machine.

## ---

**3\. Curriculum Architecture and Delivery Mechanism**

### **3.1 The "Monday-Wednesday-Friday" Micro-Learning Cadence**

Graduate students are time-poor. A traditional lecture series often sees high attrition. This course utilizes an asynchronous, email-based "drip" methodology, which aligns with the "spaced repetition" principles of learning science.

* **Monday (The Deep Dive):** A 1,500-word essay delivering the core theoretical concept and practical framework. This replaces the "lecture."  
* **Wednesday (The Micro-Challenge):** A specific, constrained task (approx. 30 minutes) requiring the application of Monday's concept. This emphasizes *process* over *product*.  
* **Friday (The Download):** A curated set of readings, tool updates (with obsolescence warnings), and a reflective prompt to consolidate the week's learning.

### **3.2 Phase Structure**

The 10-week journey is segmented into three developmental phases:

1. **Phase I: Foundations (Weeks 1-3):** Understanding the "Alien Intelligence" and establishing the rules of engagement.  
2. **Phase II: Application (Weeks 4-7):** Integrating AI into the specific stages of the research lifecycle (Literature Review, Ideation, Methods, Analysis).  
3. **Phase III: Ethics & Future (Weeks 8-10):** Addressing high-stakes issues like peer review, epistemic collapse, and long-term policy.

## ---

**4\. Phase I: Foundations of the Augmented Mind (Weeks 1-3)**

### **Week 1: Unlocking the Black Box – Probability, Not Truth**

**Pedagogical Goal:** To shatter the anthropomorphic illusion of the "smart chatbot" and replace it with the mental model of a "probabilistic token predictor."

Curricular Content:  
The inaugural week focuses on the "First Principles" of Large Language Models (LLMs). We begin by explaining tokenization—the process by which text is converted into numerical vectors.10 This explanation is vital because it demystifies why LLMs struggle with tasks that seem simple to humans (like spelling "strawberry" or doing math) while excelling at complex semantic association.  
We then explore **Next-Token Prediction** and the concept of **Temperature**. By explaining that the model is merely predicting the most statistically likely continuation of a sequence 8, we provide the structural explanation for **hallucination**. Hallucinations are not "errors" in the system's logic; they are the system functioning exactly as designed—prioritizing plausibility and coherence over factual accuracy.7 This week introduces the "Stochastic Parrot" metaphor (Bender et al.) alongside more recent nuanced views of "emergent reasoning".23

The Micro-Challenge: "The Unplugged Probability Game"  
To reinforce the concept of probabilistic generation without using a screen, students engage in an analog thought experiment.20 They are given a sentence stem (e.g., "The primary limitation of this study is...") and must list the five most probable next words, distinct from the truest next words. They then compare this to an actual LLM output. This "unplugged" activity 24 highlights how predictive text mirrors—and diverges from—human intent.  
**Resources:**

* Snippet 10: "Generative AI Foundations: From Tokens to Text."  
* Snippet 8: OpenAI's analysis on "Why Language Models Hallucinate."

### **Week 2: The Art of Inquiry – Prompt Engineering as Research Methodology**

**Pedagogical Goal:** To transition students from "asking questions" to "designing constraints," treating prompts as rigorous methodological instruments.

Curricular Content:  
This week reframes "Prompt Engineering" not as a "hack" but as a form of scientific communication. If an LLM is a probability engine, a prompt is a set of constraints designed to shape that probability distribution toward a useful output. We introduce the hierarchy of prompting techniques:

1. **Zero-Shot vs. Few-Shot:** We present evidence showing that providing examples (Few-Shot) significantly improves performance by "aligning" the model's latent space with the user's intent.25  
2. **Chain of Thought (CoT):** We delve into the seminal research 23 demonstrating that asking the model to "think step-by-step" forces it to generate intermediate reasoning tokens. This acts as a "scratchpad," allowing the model to error-correct its own logic before producing a final answer.  
3. **Persona/Role-Playing:** We discuss the utility of assigning roles (e.g., "Act as a harsh peer reviewer" or "Act as a novice undergraduate") to adjust the *tone* and *complexity* of the output.26

The Micro-Challenge: "The Prompt Tournament"  
Students select a complex research task (e.g., "Summarize this abstract for a grant committee"). They must write three versions of the prompt:

1. **The Naive Prompt:** "Summarize this."  
2. **The Contextual Prompt:** Adds role and context.  
3. The CoT Prompt: Adds reasoning steps and examples.  
   They then analyze the variance in quality, documenting how specific constraints led to specific improvements.29

**Resources:**

* Snippet 23: "Chain of Thought Prompting Elicits Reasoning in Large Language Models."  
* Snippet 37: "The Hitchhiker’s Guide to Socratic Methods in Prompting."

### **Week 3: Cognitive Ethics – Centaurs, Cyborgs, and Offloading**

**Pedagogical Goal:** To develop a personal "Cognitive Risk Policy," determining which tasks are safe to offload and which must remain human-led.

Curricular Content:  
Having learned how to use the tool, we now ask when to use it. We formally introduce the Centaur vs. Cyborg framework.1 The central tension of this week is Cognitive Offloading.3 We discuss the concept of "Desirable Difficulty"—the idea that the struggle to synthesize information is what encodes it into long-term memory. If we offload the struggle, we lose the learning.  
We present a rubric for "Safe vs. Unsafe Offloading":

* **Safe (Centaur):** Formatting, translation, code debugging, preliminary summarization (with verification).  
* **Unsafe (Full Automation):** Interpretive coding, final hypothesis generation, writing the "Discussion" section.  
* **Hybrid (Cyborg):** Brainstorming, stylistic editing, counter-argument generation.

The Micro-Challenge: "The Cognitive Audit"  
Students track their research workflow for two days. They map their tasks onto a "Jagged Frontier" chart 2, categorizing them as:

1. **"AI Advantage"** (High AI skill, low human cost).  
2. **"Human Advantage"** (Nuance required, high risk of hallucination).  
3. **"The Danger Zone"** (Tasks that *feel* efficient to offload but degrade critical thinking, e.g., reading primary sources).4

**Resources:**

* Snippet 2: "Centaurs and Cyborgs: Interacting with Artificial Intelligence Tooling."  
* Snippet 3: "AI's Cognitive Implications: The Decline of Our Thinking Skills."

## ---

**5\. Phase II: The Research Lifecycle (Weeks 4-7)**

### **Week 4: The Literature Review – Synthesis Over Search**

**Pedagogical Goal:** To differentiate between *finding* information (Retrieval) and *connecting* information (Synthesis), and to mitigate the risks of "hallucinated bibliographies."

Curricular Content:  
The literature review is perhaps the most perilous stage for GenAI use due to the high rate of citation fabrication.13 We emphasize that ChatGPT is not a search engine. We introduce Retrieval Augmented Generation (RAG) conceptually 30 to explain how tools like Perplexity or Elicit differ from raw LLMs by "grounding" their answers in retrieved documents.  
The focus, however, is on **Synthesis**. We teach a workflow where the human performs the retrieval (ensuring source validity) and the AI aids in comparison. For example, pasting *verified* abstracts into the context window and prompting: *"Compare the methodological approaches of these five papers. Create a matrix of variables."*.32 We also address the "Homogenization Risk"—the tendency of LLMs to smooth out conflicting academic voices into a bland consensus.34

The Micro-Challenge: "The Frankenstein Citation Hunt"  
Students ask a raw LLM (like GPT-4) to generate a bibliography on a niche topic. They must then audit the results to find:

* **Real Citations.**  
* **Hallucinations.**  
* "Frankensteins": Real authors and real journals, but a made-up title that sounds like something that author would write.13  
  This exercises "Epistemic Vigilance."

**Resources:**

* Snippet 32: "Generative AI for Literature Reviews."  
* Snippet 14: "ChatGPT as a Real-time Literature Search Tool: A Systematic Review."

### **Week 5: Ideation and Hypothesis – The "Hypogenic" Researcher**

**Pedagogical Goal:** To leverage AI for *divergent* thinking and hypothesis generation, using the machine as a "Sparring Partner" rather than an oracle.

Curricular Content:  
This week explores the use of LLMs for scientific hypothesis generation.35 We discuss how LLMs, trained on vast cross-disciplinary datasets, can identify latent connections between fields that a specialized human might miss. The concept of "HypoGeniC" (Hypothesis Generation in Context) 35 is adapted for a general audience.  
We introduce **Socratic Prompting** 37 as a key technique. Instead of asking the AI for answers, the researcher prompts: *"I am developing a hypothesis about \[X\]. Ask me 5 critical questions to test the robustness of my theory. Do not be agreeable; be skeptical."* This uses the AI to sharpen the human's thinking. We also cover **Adversarial Prompting** 21, where the AI is tasked with generating counter-hypotheses or identifying confounding variables the researcher ignored.

The Micro-Challenge: "The Devil's Advocate"  
Students feed a brief summary of their current research project into the AI. They utilize a specific "Reviewer \#2" persona prompt 28 to solicit a brutal critique of their logic, methodology, and theoretical assumptions. They must then write a human response defending their work against the AI's critique.  
**Resources:**

* Snippet 35: "HypoGeniC: Hypothesis Generation."  
* Snippet 37: "The Hitchhiker’s Guide to Socratic Methods."

### **Week 6: Methodological Support – Coding, Quant, and Qual**

**Pedagogical Goal:** To navigate the specific strengths and weaknesses of AI in data analysis, distinguishing between *code generation* (high value) and *interpretive coding* (high risk).

Curricular Content:  
This week splits into two tracks:

1. **Quantitative/Computational:** We explore the **"No-Code"** revolution. Researchers who do not know Python or R can now use AI to generate scripts for data cleaning and visualization.39 We emphasize the importance of reading the *code* (or testing it) rather than trusting the *output* blindly. We also touch on **Synthetic Data** generation for training models or testing pipelines.41  
2. **Qualitative:** We critically examine the use of AI for thematic analysis. Research suggests AI is effective for **deductive coding** (finding pre-defined themes) but struggles with **inductive coding** (interpreting nuance and subtext).18 We warn against the loss of "intimate familiarity" with the data 43 and propose a workflow where AI serves as a secondary check for inter-coder reliability, not the primary coder.44

**The Micro-Challenge: "The Data Sprint"**

* *Quant:* Download a messy public dataset. Use AI to write a Python script to clean it and generate a specific chart (e.g., Violin Plot). Run the script in a sandbox.  
* *Qual:* Take one interview transcript. Code it manually. Then ask AI to code it. Compare the depth and nuance. Note what the AI missed.43

**Resources:**

* Snippet 43: "Using Generative AI for Qualitative Coding."  
* Snippet 39: "No-Code Data Analytics with Generative AI."

### **Week 7: Dissemination – Writing, Voice, and Audience**

**Pedagogical Goal:** To master the use of AI for stylistic adaptation and editing while preserving authorship and "voice."

Curricular Content:  
Writing is not merely reporting; it is a mode of thinking. We discuss the ethical boundaries of AI in manuscript preparation. While most top-tier journals prohibit AI as an author, they increasingly allow it as a tool for editing and polishing.45  
We focus on **Style Transfer** and **Audience Adaptation**.47 A researcher can draft a complex technical paragraph and ask the AI: *"Rewrite this for a policy-maker audience, focusing on actionable outcomes,"* or *"Simplify the syntax for a non-native English speaker without losing technical precision."* We also caution against the "AI Voice"—the flat, overly polished, and buzzword-laden prose (e.g., "delve," "tapestry") that often signals AI generation.49

The Micro-Challenge: "The Abstract Remix"  
Students take their own abstract and use Style Transfer prompts 47 to rewrite it for three audiences:

1. An expert in a specific adjacent field.  
2. A journalist for a popular science outlet.  
3. A grant funding committee.  
   They analyze how the AI altered the vocabulary and structure for each.

**Resources:**

* Snippet 47: "AI Writing Style Adapter."  
* Snippet 48: "Adapting Writing for Diverse Academic Audiences."

## ---

**6\. Phase III: Epistemic and Ethical Horizons (Weeks 8-10)**

### **Week 8: The Peer Review Simulation – Ethics and Utility**

**Pedagogical Goal:** To use AI to *prepare* for peer review, while strictly avoiding the unethical use of AI to *perform* peer review.

Curricular Content:  
Peer review is the gatekeeper of scientific integrity. We discuss the emerging scandal of "hidden prompts" in published papers 50, where reviewers clearly pasted manuscripts into AI and copy-pasted the output. This is a profound ethical breach involving confidentiality and intellectual laziness.  
However, we *can* use AI ethically as a "Pre-Submission Stress Test." We teach students to prompt the AI with the specific rubric of their target journal. *"Act as a reviewer for \[Journal Name\]. Evaluate this Introduction against the criteria of novelty and fit."*.28 This allows authors to anticipate critiques. We also discuss the limitations: AI tends to be overly agreeable or focus on surface-level structure rather than deep theoretical flaws.18

The Micro-Challenge: "Reviewing the Reviewer"  
Students submit a section of their draft to an AI "Reviewer." They are tasked with grading the AI's feedback. Did it identify the actual weak point? Did it hallucinate a flaw? This reinforces the human's role as the final arbiter of quality.52  
**Resources:**

* Snippet 50: "Scientists Reportedly Hiding AI Text Prompts."  
* Snippet 28: "Roleplaying with GenAI."

### **Week 9: Epistemic Security – Model Collapse and the Future of Truth**

**Pedagogical Goal:** To understand the macro-level risks of AI to the scientific record and the individual researcher's duty to maintain "Epistemic Security."

Curricular Content:  
This week zooms out to the systemic risks. We explore Model Collapse 5—the theory that as the internet floods with AI-generated content, future models trained on this "synthetic sludge" will degrade, losing the nuance and "long tail" of human knowledge. This is the "Ouroboros" effect.53  
We discuss the **Pollution of the Scientific Record** via AI-generated paper mills.54 The lesson for the graduate student is clear: **Human verification is the new premium.** In an age of abundant synthetic text, the unique value of a researcher lies in their ability to generate *verified*, *novel*, and *human-grounded* insight. We frame "inefficient" human processes (like reading a book cover-to-cover) as essential "Epistemic Hygiene".56

The Micro-Challenge: "The Turing Test for Papers"  
Students are presented with two abstracts (one real, one AI-generated). They must identify the AI based on stylistic cues (lack of concrete data, vague methodology, "hallucinated" confidence). This trains their "BS detector".13  
**Resources:**

* Snippet 5: "Epistemic Risk and Model Collapse."  
* Snippet 56: "Global Knowledge Collapse."

### **Week 10: Governance – Designing Your Personal AI Manifesto**

**Pedagogical Goal:** To codify the course learnings into a sustainable, personal code of ethics and practice.

Curricular Content:  
Institutions are moving slowly; researchers must move fast. We review various university policies (Columbia, Harvard, Arizona) to see the landscape of regulation.58 We note the common threads: Accountability (you are responsible for the output), Transparency (you must disclose use), and Privacy (no sensitive data in the machine).61  
The final module guides students to create their own **"Personal AI Policy"** or **"Lab Manifesto."** This document defines their "Red Lines" (e.g., "I will never use AI to write the Discussion section") and their "Green Zones" (e.g., "I will always use AI to check code syntax"). This transforms the "Centaur" methodology from a theory into a daily practice.16

The Micro-Challenge: "The Manifesto Draft"  
Students draft a 1-page "AI Disclosure Statement" suitable for appending to a thesis or dissertation. It details exactly how AI was used (and not used) in their work, serving as a model for transparency.62  
**Resources:**

* Snippet 62: "APUS Generative AI Policy."  
* Snippet 58: "Syllabus Policy Statements."

## ---

**7\. Implementation & Resource Curation**

### **7.1 The "Living" Resource Repository**

To avoid the "outdated tool" trap, the course will maintain a "Living Repository" (e.g., a Notion page or GitHub repo) referenced in the Friday emails. This repository separates **Concepts** (permanent) from **Tools** (transient).

* **Concept:** "Retrieval Augmented Generation" (Permanent).  
* **Tool:** "Consensus.app," "Elicit.org," "Perplexity" (Transient – tagged with "Current as of").

### **7.2 Assessment of Learning**

Success in this course is not measured by a final exam, but by the **evolution of the researcher's workflow**. The primary metric is the sophistication of the "Personal Manifesto" produced in Week 10\.

* *Baseline:* "I use ChatGPT to fix my grammar."  
* *Mastery:* "I use a Chain-of-Thought prompt structure to simulate peer review critiques, but I retain full control over the inductive coding of my qualitative data to prevent homogenization of themes."

### **7.3 Risk Mitigation Strategy**

The course explicitly addresses the "Shadow Syllabus"—the unethical uses students might discover on their own. By bringing topics like "hiding prompts" 50 and "fabricating data" 54 into the light, we strip them of their illicit appeal and frame them as professional liabilities. We emphasize that in a small academic community, reputation is fragile, and the "AI stain" of a retracted, hallucinated paper is a career-ending event.55

## ---

**8\. Conclusion: The Sovereign Researcher**

The trajectory of this 10-week curriculum is a movement from **Anxiety** to **Agency**. Many graduate students currently fear that AI will render their labor obsolete. By mastering the "Jagged Frontier" and adopting the "Centaur" mindset, they learn that AI is not a replacement for the scholar, but a powerful **cognitive exoskeleton**.

However, this exoskeleton requires a strong spine. The course concludes with the assertion that the "Augmented Academic" must be *more* rigorous, *more* ethical, and *more* human than their predecessors. In a world of cheap, synthetic generation, the rigorous verification of truth becomes the ultimate luxury good—and the defining duty of the scientist.

## ---

**9\. Appendix: Select Curricular Tables**

### **Table 2: Risk Matrix for Research Stages (Week 3\)**

| Research Stage | AI Utility (Potential) | Epistemic Risk | Recommended Approach |
| :---- | :---- | :---- | :---- |
| **Lit Review** | High (Synthesis, Mapping) | **Critical** (Hallucination) | **Centaur:** Human finds papers; AI synthesizes them. |
| **Ideation** | Very High (Divergent thinking) | Low (Brainstorming is safe) | **Cyborg:** Rapid back-and-forth dialogue. |
| **Data Collection** | Moderate (Synthetic Data) | **High** (Bias, Privacy) | **Human-Led:** AI used only for scripting/logistics. |
| **Analysis (Quant)** | High (Code Generation) | Moderate (Logic errors) | **Centaur:** AI writes code; Human verifies/runs it. |
| **Analysis (Qual)** | Moderate (Deductive coding) | **High** (Loss of nuance) | **Human-Led:** AI used for secondary reliability check. |
| **Writing** | High (Editing, Formatting) | Moderate (Loss of Voice) | **Cyborg:** Iterative drafting with heavy human editing. |

### **Table 3: Prompt Engineering Anatomy (Week 2\)**

| Component | Function | Example Snippet |
| :---- | :---- | :---- |
| **Persona** | Sets the tone and expertise level. | "Act as a senior biostatistician..." |
| **Context** | Grounds the probability distribution. | "I am analyzing a small dataset (n=50) of..." |
| **Task** | Defines the explicit goal. | "Suggest three non-parametric tests..." |
| **Constraint** | Limits the search space. | "Do not suggest Bayesian methods." |
| **Format** | Structures the output for usability. | "Output as a Markdown table." |
| **Reasoning (CoT)** | Reduces logic errors. | "Explain the assumptions of each test step-by-step." |

*(End of Report)*

#### **Works cited**

1. Humans vs. Machines: Untangling the Tasks AI Can (and Can't) Handle \- Baker Library, accessed December 19, 2025, [https://www.library.hbs.edu/working-knowledge/humans-vs-machines-untangling-the-tasks-ai-can-and-cant-handle](https://www.library.hbs.edu/working-knowledge/humans-vs-machines-untangling-the-tasks-ai-can-and-cant-handle)  
2. Centaurs and Cyborgs: Interacting with Artificial Intelligence Tooling \- Eric Ma, accessed December 19, 2025, [https://ericmjl.github.io/blog/2023/9/17/centaurs-and-cyborgs-interacting-with-artificial-intelligence-tooling/](https://ericmjl.github.io/blog/2023/9/17/centaurs-and-cyborgs-interacting-with-artificial-intelligence-tooling/)  
3. AI's cognitive implications: the decline of our thinking skills? \- IE, accessed December 19, 2025, [https://www.ie.edu/center-for-health-and-well-being/blog/ais-cognitive-implications-the-decline-of-our-thinking-skills/](https://www.ie.edu/center-for-health-and-well-being/blog/ais-cognitive-implications-the-decline-of-our-thinking-skills/)  
4. AI Tools in Society: Impacts on Cognitive Offloading and the Future of Critical Thinking, accessed December 19, 2025, [https://www.mdpi.com/2075-4698/15/1/6](https://www.mdpi.com/2075-4698/15/1/6)  
5. Epistemic diversity across language models mitigates knowledge collapse \- arXiv, accessed December 19, 2025, [https://arxiv.org/html/2512.15011v1](https://arxiv.org/html/2512.15011v1)  
6. AI models collapse when trained on recursively generated data \- PMC \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC11269175/](https://pmc.ncbi.nlm.nih.gov/articles/PMC11269175/)  
7. LLM Hallucinations Explained. LLMs like the GPT family, Claude… | by Nirdiamant | Medium, accessed December 19, 2025, [https://medium.com/@nirdiamant21/llm-hallucinations-explained-8c76cdd82532](https://medium.com/@nirdiamant21/llm-hallucinations-explained-8c76cdd82532)  
8. Why language models hallucinate \- OpenAI, accessed December 19, 2025, [https://openai.com/index/why-language-models-hallucinate/](https://openai.com/index/why-language-models-hallucinate/)  
9. Teaching-AI-Best-Practices.pdf \- AI | University of Florida, accessed December 19, 2025, [https://ai.ufl.edu/media/aiufledu/ai-research/Teaching-AI-Best-Practices.pdf](https://ai.ufl.edu/media/aiufledu/ai-research/Teaching-AI-Best-Practices.pdf)  
10. Generative AI Foundations : From Tokens to Text, How LLMs “Write” \- Medium, accessed December 19, 2025, [https://medium.com/generative-ai-playbook/generative-ai-foundations-from-tokens-to-text-how-llms-write-05f1800703ab](https://medium.com/generative-ai-playbook/generative-ai-foundations-from-tokens-to-text-how-llms-write-05f1800703ab)  
11. Explaining Tokens — the Language and Currency of AI \- NVIDIA Blog, accessed December 19, 2025, [https://blogs.nvidia.com/blog/ai-tokens-explained/](https://blogs.nvidia.com/blog/ai-tokens-explained/)  
12. An Introduction to Generative Artificial Intelligence for Academics. \- F1000Research, accessed December 19, 2025, [https://f1000research.com/articles/14-655](https://f1000research.com/articles/14-655)  
13. Investigating generative AI models and detection techniques: impacts of tokenization and dataset size on identification of AI-generated text \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC11611853/](https://pmc.ncbi.nlm.nih.gov/articles/PMC11611853/)  
14. The Use of Generative AI for Scientific Literature Searches for Systematic Reviews: ChatGPT and Microsoft Bing AI Performance Evaluation \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC11107769/](https://pmc.ncbi.nlm.nih.gov/articles/PMC11107769/)  
15. Centaurs vs. Cyborgs \- Profitable AI Weekly, accessed December 19, 2025, [https://blog.tobiaszwingmann.com/p/generative-ai-centaurs-vs-cyborgs](https://blog.tobiaszwingmann.com/p/generative-ai-centaurs-vs-cyborgs)  
16. How to Pick the Right AI Strategy: Cyborg vs Centaur \- Mind Map Nation, accessed December 19, 2025, [https://www.mindmapnation.com/epiphany/how-to-pick-the-right-ai-strategy-cyborg-vs-centaur](https://www.mindmapnation.com/epiphany/how-to-pick-the-right-ai-strategy-cyborg-vs-centaur)  
17. Cognitive processes while using Artificial Intelligence at work: a research agenda on challenges and opportunities Processi cogn, accessed December 19, 2025, [https://oaj.fupress.net/index.php/formare/article/download/17122/13856/80903](https://oaj.fupress.net/index.php/formare/article/download/17122/13856/80903)  
18. Comparing the Efficacy and Efficiency of Human and Generative AI: Qualitative Thematic Analyses \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/11329846/](https://pmc.ncbi.nlm.nih.gov/articles/11329846/)  
19. AI Unplugged, accessed December 19, 2025, [https://www.aiunplugged.org/](https://www.aiunplugged.org/)  
20. 3 Unplugged Activities for Teaching About AI \- ISTE, accessed December 19, 2025, [https://iste.org/blog/3-unplugged-activities-for-teaching-about-ai](https://iste.org/blog/3-unplugged-activities-for-teaching-about-ai)  
21. A Survey on Hypothesis Generation for Scientific Discovery in the Era of Large Language Models \- arXiv, accessed December 19, 2025, [https://arxiv.org/html/2504.05496v1](https://arxiv.org/html/2504.05496v1)  
22. LLM Hallucinations 101: Why Do They Appear? Can We Avoid Them?, accessed December 19, 2025, [https://neptune.ai/blog/llm-hallucinations](https://neptune.ai/blog/llm-hallucinations)  
23. What is chain of thought (CoT) prompting? \- IBM, accessed December 19, 2025, [https://www.ibm.com/think/topics/chain-of-thoughts](https://www.ibm.com/think/topics/chain-of-thoughts)  
24. AI Unplugged | Low-tech, hands-on activities to engage youth in learning about AI, accessed December 19, 2025, [https://sites.northwestern.edu/aiunplugged/](https://sites.northwestern.edu/aiunplugged/)  
25. Few-Shot Prompting \- Prompt Engineering Guide, accessed December 19, 2025, [https://www.promptingguide.ai/techniques/fewshot](https://www.promptingguide.ai/techniques/fewshot)  
26. Effective Prompts for AI: The Essentials \- MIT Sloan Teaching & Learning Technologies, accessed December 19, 2025, [https://mitsloanedtech.mit.edu/ai/basics/effective-prompts/](https://mitsloanedtech.mit.edu/ai/basics/effective-prompts/)  
27. Chain-of-thought prompting: When and why to use it (with examples that actually show the difference) : r/ChatGPTPromptGenius \- Reddit, accessed December 19, 2025, [https://www.reddit.com/r/ChatGPTPromptGenius/comments/1ppwgyr/chainofthought\_prompting\_when\_and\_why\_to\_use\_it/](https://www.reddit.com/r/ChatGPTPromptGenius/comments/1ppwgyr/chainofthought_prompting_when_and_why_to_use_it/)  
28. Roleplaying with GenAI \- The Peer Review, accessed December 19, 2025, [https://thepeerreview-iwca.org/issues/issue-9-1/roleplaying-with-genai/](https://thepeerreview-iwca.org/issues/issue-9-1/roleplaying-with-genai/)  
29. Mastering AI-Powered Research: My Guide to Deep Research, Prompt Engineering, and Multi-Step Workflows : r/ChatGPTPro \- Reddit, accessed December 19, 2025, [https://www.reddit.com/r/ChatGPTPro/comments/1in87ic/mastering\_aipowered\_research\_my\_guide\_to\_deep/](https://www.reddit.com/r/ChatGPTPro/comments/1in87ic/mastering_aipowered_research_my_guide_to_deep/)  
30. A Comprehensive Survey of Hallucination Mitigation Techniques in Large Language Models, accessed December 19, 2025, [https://arxiv.org/html/2401.01313v2](https://arxiv.org/html/2401.01313v2)  
31. 7 Techniques to Reduce AI Errors & Improve Responses | by Tahir | Medium, accessed December 19, 2025, [https://medium.com/@tahirbalarabe2/7-techniques-to-reduce-ai-errors-improve-responses-59588b69c0ba](https://medium.com/@tahirbalarabe2/7-techniques-to-reduce-ai-errors-improve-responses-59588b69c0ba)  
32. Adopting Generative AI for Literature Reviews: An Epistemological Perspective \- Semantic Scholar, accessed December 19, 2025, [https://pdfs.semanticscholar.org/e6e7/4f14ad60267e7fe1c7bb98b406494a1bdb83.pdf](https://pdfs.semanticscholar.org/e6e7/4f14ad60267e7fe1c7bb98b406494a1bdb83.pdf)  
33. Is Utilizing AI Tools for Conducting Literature Reviews in Academic Research Advisable?, accessed December 19, 2025, [https://academia.stackexchange.com/questions/205889/is-utilizing-ai-tools-for-conducting-literature-reviews-in-academic-research-adv](https://academia.stackexchange.com/questions/205889/is-utilizing-ai-tools-for-conducting-literature-reviews-in-academic-research-adv)  
34. Response to Open Letter that Opposes the Use of Generative AI for Reflexive Qualitative Research \- Qeludra Blog, accessed December 19, 2025, [https://qeludra.com/blog/response-to-open-letter-opposing-the-use-of-generative-ai-for-reflexive-qualitative-research](https://qeludra.com/blog/response-to-open-letter-opposing-the-use-of-generative-ai-for-reflexive-qualitative-research)  
35. Hypothesis generation project, accessed December 19, 2025, [https://chicagohai.github.io/hypogenic-demo/](https://chicagohai.github.io/hypogenic-demo/)  
36. Scientific hypothesis generation by large language models: laboratory validation in breast cancer treatment \- PMC \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC12134935/](https://pmc.ncbi.nlm.nih.gov/articles/PMC12134935/)  
37. The Hitchhiker's Guide to Socratic Methods in Prompting Large Language Models for Chemistry Applications \- ChemRxiv, accessed December 19, 2025, [https://chemrxiv.org/engage/api-gateway/chemrxiv/assets/orp/resource/item/67a236fc6dde43c90892cf6f/original/the-hitchhiker-s-guide-to-socratic-methods-in-prompting-large-language-models-for-chemistry-applications.pdf](https://chemrxiv.org/engage/api-gateway/chemrxiv/assets/orp/resource/item/67a236fc6dde43c90892cf6f/original/the-hitchhiker-s-guide-to-socratic-methods-in-prompting-large-language-models-for-chemistry-applications.pdf)  
38. Socratic Question Generation: A Novel Dataset, Models, and Evaluation \- ACL Anthology, accessed December 19, 2025, [https://aclanthology.org/2023.eacl-main.12.pdf](https://aclanthology.org/2023.eacl-main.12.pdf)  
39. No-Code Data Analytics with Generative AI \- Stanford University, accessed December 19, 2025, [https://uit.stanford.edu/service/techtraining/class/no-code-data-analytics-generative-ai](https://uit.stanford.edu/service/techtraining/class/no-code-data-analytics-generative-ai)  
40. No Code AI and Machine Learning: Building Data Science Solutions, accessed December 19, 2025, [https://professional.mit.edu/course-catalog/no-code-ai-and-machine-learning-building-data-science-solutions](https://professional.mit.edu/course-catalog/no-code-ai-and-machine-learning-building-data-science-solutions)  
41. A Systematic Review of Synthetic Data Generation Techniques Using Generative AI \- MDPI, accessed December 19, 2025, [https://www.mdpi.com/2079-9292/13/17/3509](https://www.mdpi.com/2079-9292/13/17/3509)  
42. Synthetic Data Sets: Data Generation for Machine Learning \- Coursera, accessed December 19, 2025, [https://www.coursera.org/articles/synthetic-datasets](https://www.coursera.org/articles/synthetic-datasets)  
43. (PDF) Using Generative AI for Qualitative Coding \- ResearchGate, accessed December 19, 2025, [https://www.researchgate.net/publication/392174927\_Using\_Generative\_AI\_for\_Qualitative\_Coding](https://www.researchgate.net/publication/392174927_Using_Generative_AI_for_Qualitative_Coding)  
44. Lessons from a pilot study on AI coding and analysis of qualitative patient data, accessed December 19, 2025, [https://becarispublishing.com/digital-content/blog-post/lessons-pilot-study-ai-coding-and-analysis-qualitative-patient-data](https://becarispublishing.com/digital-content/blog-post/lessons-pilot-study-ai-coding-and-analysis-qualitative-patient-data)  
45. Risks and Limitations of Generative AI in Research and Creative Activities, accessed December 19, 2025, [https://research.msu.edu/generative-ai/risk-limitations](https://research.msu.edu/generative-ai/risk-limitations)  
46. Ten simple rules for optimal and careful use of generative AI in science \- PMC \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC12561928/](https://pmc.ncbi.nlm.nih.gov/articles/PMC12561928/)  
47. Adapt your text to different writing styles | HyperWrite AI Writing Assistant, accessed December 19, 2025, [https://www.hyperwriteai.com/aitools/ai-writing-style-adapter](https://www.hyperwriteai.com/aitools/ai-writing-style-adapter)  
48. StudyPro Introduces AI-Powered Guidance To Help Students Adapt Writing For Diverse Academic Audiences \- Barchart.com, accessed December 19, 2025, [https://www.barchart.com/story/news/34554020/studypro-introduces-ai-powered-guidance-to-help-students-adapt-writing-for-diverse-academic-audiences](https://www.barchart.com/story/news/34554020/studypro-introduces-ai-powered-guidance-to-help-students-adapt-writing-for-diverse-academic-audiences)  
49. AI in Academic Writing \- Clemson University, accessed December 19, 2025, [https://www.clemson.edu/centers-institutes/writing/writing-resources/writing-resources/ai-in-academic-writing.html](https://www.clemson.edu/centers-institutes/writing/writing-resources/writing-resources/ai-in-academic-writing.html)  
50. Scientists reportedly hiding AI text prompts in academic papers to receive positive peer reviews | Artificial intelligence (AI) : r/technology \- Reddit, accessed December 19, 2025, [https://www.reddit.com/r/technology/comments/1lzc65y/scientists\_reportedly\_hiding\_ai\_text\_prompts\_in/](https://www.reddit.com/r/technology/comments/1lzc65y/scientists_reportedly_hiding_ai_text_prompts_in/)  
51. Peer Review: Make peer feedback easy, effective, and reliable \- FeedbackFruits, accessed December 19, 2025, [https://feedbackfruits.com/solutions/peer-review](https://feedbackfruits.com/solutions/peer-review)  
52. Personal experience with AI-generated peer reviews: a case study \- PMC \- NIH, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC11974187/](https://pmc.ncbi.nlm.nih.gov/articles/PMC11974187/)  
53. accessed December 19, 2025, [https://www.vktr.com/ai-technology/model-collapse-how-generative-ai-is-eating-its-own-data/\#:\~:text=Model%20collapse%20occurs%20when%20generative,over%20lived%20experience%20or%20fact.](https://www.vktr.com/ai-technology/model-collapse-how-generative-ai-is-eating-its-own-data/#:~:text=Model%20collapse%20occurs%20when%20generative,over%20lived%20experience%20or%20fact.)  
54. GenAI synthetic data create ethical challenges for scientists. Here's how to address them, accessed December 19, 2025, [https://pmc.ncbi.nlm.nih.gov/articles/PMC11892638/](https://pmc.ncbi.nlm.nih.gov/articles/PMC11892638/)  
55. Managing Opportunities and Risks in Generative AI Use for Clinical Research \- PPD, accessed December 19, 2025, [https://www.ppd.com/blog/managing-opportunities-risks-generative-ai-clinical-research/](https://www.ppd.com/blog/managing-opportunities-risks-generative-ai-clinical-research/)  
56. What AI doesn't know: we could be creating a global 'knowledge collapse' | Artificial intelligence (AI) | The Guardian, accessed December 19, 2025, [https://www.theguardian.com/news/2025/nov/18/what-ai-doesnt-know-global-knowledge-collapse](https://www.theguardian.com/news/2025/nov/18/what-ai-doesnt-know-global-knowledge-collapse)  
57. Epistemic Collapse in the Age of AI-Generated Hyperreality | by Lauri Korpela \- Medium, accessed December 19, 2025, [https://medium.com/epistemic-security-studies/epistemic-collapse-in-the-age-of-ai-generated-hyperreality-79fc179497df](https://medium.com/epistemic-security-studies/epistemic-collapse-in-the-age-of-ai-generated-hyperreality-79fc179497df)  
58. ChatGPT and Generative AI Tools: Sample Syllabus Policy Statements | Center for Teaching & Learning \- The University of Texas at Austin, accessed December 19, 2025, [https://ctl.utexas.edu/chatgpt-and-generative-ai-tools-sample-syllabus-policy-statements](https://ctl.utexas.edu/chatgpt-and-generative-ai-tools-sample-syllabus-policy-statements)  
59. Guidelines for Syllabus Statements About Generative AI \- UCATT \- The University of Arizona, accessed December 19, 2025, [https://ucatt.arizona.edu/sites/default/files/2023-08/Syllabus-Guidance-2.1.1.pdf](https://ucatt.arizona.edu/sites/default/files/2023-08/Syllabus-Guidance-2.1.1.pdf)  
60. Generative AI Policy | Office of the Provost \- Columbia University, accessed December 19, 2025, [https://provost.columbia.edu/content/office-senior-vice-provost/ai-policy](https://provost.columbia.edu/content/office-senior-vice-provost/ai-policy)  
61. Generative AI Guidelines | Harvard University Information Technology, accessed December 19, 2025, [https://www.huit.harvard.edu/ai/guidelines](https://www.huit.harvard.edu/ai/guidelines)  
62. Generative AI Policy | American Public University, accessed December 19, 2025, [https://www.apu.apus.edu/student-handbook/university-policies-and-code-of-conduct/apus-student-code-of-conduct/generative-ai-policy/](https://www.apu.apus.edu/student-handbook/university-policies-and-code-of-conduct/apus-student-code-of-conduct/generative-ai-policy/)

# **Claude report**

# **Designing a 10-Week Email Course on Generative AI in Academic Research**

Researchers need AI literacy training that builds transferable skills and critical judgment rather than tool proficiency that quickly becomes obsolete. This comprehensive research synthesis reveals a mature ecosystem of educational frameworks, competency models, and practical applications that can inform a principled approach to AI education for scholars. The evidence strongly supports a course structure that progresses from foundational understanding through critical evaluation to independent, reflective practice—with ethics and metacognition woven throughout rather than siloed.

The landscape has evolved rapidly since 2022, with **UNESCO, EDUCAUSE, and Stanford all releasing competency frameworks** emphasizing that effective AI literacy requires cognitive, ethical, and metacognitive skills working together. Research consistently shows that structured training with reflection outperforms unstructured exploration, and that human-AI collaboration skills transfer across tools when grounded in principles rather than procedures.

---

## **The evidence base reveals five essential curriculum pillars**

Research across educational resources, competency frameworks, and pedagogical literature identifies five interconnected domains that any comprehensive AI literacy curriculum must address. These aren't sequential topics but rather interlocking competencies that should be developed in parallel throughout the course.

**Technical understanding** forms the foundation—not expertise in building AI systems, but functional knowledge of how large language models work, why they produce hallucinations, and what inherent limitations stem from their architecture. Laupichler et al. (2023) define AI literacy as "the ability to understand, use, monitor, and critically reflect on AI applications without necessarily being able to develop AI models themselves." This distinguishes the goal from computer science training.

**Critical evaluation skills** emerge as the most emphasized competency across all frameworks reviewed. Every major framework—UNESCO, Digital Promise, Stanford, EDUCAUSE—places critical assessment of AI outputs at the center. Empirical research reveals a troubling finding: a 2025 study in *Societies* found "significant negative correlation between frequent AI tool usage and critical thinking abilities." This underscores why the course must explicitly develop evaluation skills rather than assuming they'll emerge naturally from use.

**Ethical reasoning** permeates all frameworks as non-negotiable. The consensus is striking: across all major publishers and professional organizations, **AI cannot be listed as an author**, disclosure is universally required, and human accountability is absolute. But beyond compliance, researchers need frameworks for navigating genuinely contested questions about appropriate use at different research stages.

**Metacognitive awareness** receives growing attention as essential for avoiding passive AI use. ACM CHI 2024 research identifies substantial "metacognitive demands" in AI collaboration: goal articulation, task decomposition, output evaluation, and delegation decisions. Research from the British Journal of Educational Technology demonstrates that metacognitive scaffolding reduces cognitive load and improves outcomes. The course should build habits of planning, monitoring, and reflecting on AI interactions.

**Practical application skill** connects everything to actual research practice. The literature distinguishes between well-established applications (literature discovery, code debugging, writing refinement) and experimental ones (qualitative coding, survey simulation). Researchers need to understand this landscape to make informed decisions about where AI can help and where it introduces unacceptable risks.

---

## **Pedagogical principles should guide the email format**

Research on teaching transferable AI skills offers clear guidance applicable to asynchronous, self-paced learning. The optimal balance across multiple studies suggests approximately **30% conceptual foundation, 50% guided practice, and 20% reflection and transfer activities** within each learning module.

The scaffolding research recommends a four-tier progression model moving from foundational awareness through applied problem-solving to critical evaluation and finally ethical advocacy. The K. Patricia Cross Academy describes this as developing learners who become "thoughtful drivers of AI collaboration rather than passive users." For a 10-week course, this translates to early weeks establishing safe experimentation space, middle weeks developing critical evaluation capabilities, and final weeks building toward independent, principled practice.

Adult learning theory (andragogy) provides additional guidance particularly relevant for researchers across career stages. Adults learn best through direct experience with real problems, need to understand relevance to their goals, and benefit from control over their learning process. This supports designing exercises around participants' own research questions and data wherever possible.

**Metacognition should be explicitly developed**, not assumed. Research identifies three key practices: planning (setting intentions before AI interactions), monitoring (tracking effectiveness during use), and reflecting (evaluating outcomes after). Each week's email should include structured prompts for all three phases. The University of Michigan's "troubleshooting journals" and "self-reflective comments" techniques translate well to email format.

The research consistently warns against unstructured exploration. A Stanford study found that direct instruction produced marked increases in AI literacy, "particularly in the domain of knowing and understanding AI." The email course should provide clear instruction on concepts before asking participants to experiment.

---

## **Practical applications vary in maturity and risk**

The research reveals a clear hierarchy of application areas by evidence base and reliability, which should inform how each is introduced in the course.

**Literature discovery and review** represents the most mature application area. Specialized tools like Elicit, Consensus, and Semantic Scholar demonstrate **98.4% accuracy for abstract screening** in systematic review case studies, with time savings exceeding 75% for initial coding tasks. However, general chatbots like ChatGPT regularly hallucinate citations—a critical distinction to teach. The key skill is selecting appropriate tools for specific tasks and always verifying AI-generated references.

**Code writing and debugging** for R, Python, and statistical software shows strong evidence of effectiveness for common tasks. Tools like RTutor.ai translate natural language to executable code with reasonable accuracy. The crucial caveat: code may run without errors but produce incorrect results. Researchers need domain knowledge to validate outputs, making this an augmentation rather than automation application.

**Academic writing support** is widely used but requires nuanced guidance. AI excels at improving clarity, generating alternative phrasings, and overcoming writer's block. It fails at producing publication-ready scholarly content, generating accurate citations, or capturing a researcher's unique voice. The course should position AI as an editorial assistant for polishing researcher-generated content, not a ghostwriter.

**Qualitative data analysis** remains controversial and should be treated as experimental. Research shows AI can perform keyword detection and surface-level categorization, but ChatGPT generates "more literal/descriptive codes vs. researcher's latent/interpretive codes." Morgan (2023) positions AI as an "assistant in earlier phases of interpretive process" only. The epistemological tensions with reflexive qualitative traditions need explicit discussion.

**Survey simulation with "silicon samples"** offers intriguing possibilities for pretesting but raises significant concerns. AI can simulate responses correlating 0.86 with human responses, but research finds **34% of online survey participants now report using LLMs to answer open-ended questions**—potentially contaminating actual data collection. This emerging risk deserves dedicated attention.

---

## **Ethics frameworks have achieved substantial consensus**

The ethical landscape has matured considerably, with clear consensus on core principles and active debate on implementation details. The course can teach established norms while helping participants navigate contested areas.

**Universal requirements across major publishers include**: AI cannot be an author (COPE, ICMJE, and all major publishers agree), disclosure of AI use is mandatory, human accountability is non-negotiable, and verification of all AI outputs is essential. These aren't evolving guidelines—they're settled expectations.

**Documentation standards are converging** toward requiring disclosure in Methods or Acknowledgements sections, specifying the tool name, version, and date of use, describing what task AI performed, and noting which sections contain AI-assisted content. Springer Nature exempts "AI-assisted copy editing" from disclosure, while The Lancet restricts AI to "readability and language improvement only."

**Reproducibility presents genuine challenges** given that LLM outputs are probabilistic and version-dependent. Less than one-third of AI research is reproducible according to recent surveys, with 70% of AI researchers struggling to reproduce others' results. The course should teach practical documentation practices: archiving prompts, timestamping interactions, and noting model versions.

**Bias considerations specific to research contexts** include AI detectors showing bias against non-native English speakers, training data underrepresenting certain populations, and potential amplification of existing scholarly biases. The NIST AI Risk Management Framework provides a lifecycle approach to bias identification that can be adapted for research contexts.

For human subjects research, HHS/OHRP recommendations require assessing whether AI use triggers IRB considerations, ensuring adequate consent for AI processing of data, and monitoring for group harms from profiling or bias. The Belmont principles—respect for persons, beneficence, and justice—apply to AI-mediated research in ways the course should explore.

---

## **Existing resources reveal gaps this course can fill**

The research identified substantial educational resources but also clear gaps. University library guides provide excellent practical orientation but rarely address methodology or discipline-specific applications. PhD programs at Cambridge, Harvard Medical School, and George Washington integrate AI training but focus on technical fields or specific applications rather than general researcher competencies.

The **most significant gap is discipline-specific guidance for social and behavioral sciences**. Most resources are either general or STEM-focused, with limited attention to qualitative methods, survey research, or the interpretive traditions central to these fields. Resources for mid-career researchers transitioning to AI-enhanced methods are also sparse.

Several resources merit attention as models. The **Johns Hopkins Applied Generative AI Certificate** offers comprehensive hands-on training with industry tools. **FOSTER (Facilitate Open Science Training for European Research)** provides discipline-specific open science resources including social sciences content. The **UNESCO AI Competency Framework** establishes global standards with three progression levels (Acquire, Deepen, Create) and five dimensions that could structure course progression.

The **Center for Open Science** has launched initiatives benchmarking AI's ability to replicate, evaluate, and generate research—directly relevant to reproducibility and open science values the course should emphasize.

---

## **Proposed 10-week structure with sequencing rationale**

Based on the research synthesis, the following structure moves from foundations through application to independent practice, with ethics and metacognition integrated throughout rather than isolated.

### **Week 1: Foundations of human-AI collaboration in research**

**Core content**: How large language models work (training data, prediction mechanics, limitations), the landscape of AI tools for researchers, and establishing a personal framework for when and how to use AI. Introduce the planning-monitoring-reflecting cycle that will structure all exercises.

**Exercise**: AI autobiography—document current AI use, comfort level, and questions. Try a simple prompt across 2-3 tools; compare outputs and reflect on differences.

**Mid-week content**: Quick guide to accessing institutional AI tools; overview of publisher policies relevant to participants' fields.

**Rationale**: Establishes baseline, creates safe experimentation space, introduces metacognitive structure.

### **Week 2: Critical evaluation as core competency**

**Core content**: Why AI produces hallucinations, fabricates citations, and generates confident errors. Techniques for verification and validation. The "hermeneutic of suspicion"—treating AI output with the same scrutiny as any source.

**Exercise**: Citation verification challenge—request literature summary from ChatGPT on a topic in your field; verify every citation. Document hallucination patterns. Compare results with academic AI tools (Elicit, Consensus).

**Mid-week content**: Checklist for evaluating AI outputs; common hallucination patterns to watch for.

**Rationale**: Critical evaluation is the most emphasized competency across all frameworks; establishing this early prevents naive AI adoption.

### **Week 3: Prompt engineering as communication skill**

**Core content**: Principles of effective prompting (clarity, context, constraints), structured techniques (few-shot prompting, chain prompting, the CLEAR framework), and iterative refinement strategies. Frame prompting as a skill in articulating goals and decomposing tasks—transferable beyond any specific tool.

**Exercise**: Prompt iteration exercise—take a research task you're currently working on, develop increasingly refined prompts, and document how outputs change. Reflect on what made prompts more effective.

**Mid-week content**: Prompt templates for common research tasks; examples of prompts that work vs. don't work.

**Rationale**: Empirical research shows structured prompt training significantly improves outcomes; this positions prompting as communication skill rather than technical trick.

### **Week 4: AI for literature discovery and synthesis**

**Core content**: Landscape of literature search tools (Elicit, Consensus, Semantic Scholar, Research Rabbit), their capabilities and limitations. How to integrate AI into systematic review workflows while maintaining rigor. Documentation requirements for methodological transparency.

**Exercise**: Literature discovery comparison—use AI tools and traditional database search for the same research question; compare coverage, accuracy, and efficiency. Create a workflow that combines strengths of each.

**Mid-week content**: Tool comparison matrix; sample methods section language for AI-assisted literature reviews.

**Rationale**: Literature work is well-established application area with strong evidence base; practical skills transfer across tools.

### **Week 5: Ethics, transparency, and professional norms**

**Core content**: Publisher policies and disclosure requirements, the universal prohibition on AI authorship, documentation standards for reproducibility. Reflection frameworks for assessing appropriate use. The APA ethics principles (beneficence, integrity, justice) applied to AI use.

**Exercise**: Create personal disclosure template adapted for your institution and primary publication venues. Apply reflection framework to three recent or planned AI uses; assess alignment with professional norms.

**Mid-week content**: Summary of major publisher policies; sample disclosure statements.

**Rationale**: Mid-course position allows ethics to be informed by practical experience from earlier weeks while framing remaining topics.

### **Week 6: AI for academic writing—support, not substitution**

**Core content**: Appropriate uses (clarity improvement, structure feedback, overcoming blocks) vs. inappropriate uses (generating arguments, drafting core content). The "composite voice" problem—why AI produces generic prose. Techniques for using AI as editorial collaborator while maintaining authorial voice.

**Exercise**: Writing refinement workshop—take a paragraph from work in progress, get AI feedback on clarity and structure, implement suggestions, then evaluate which feedback improved the work. Reflect on what AI couldn't see.

**Mid-week content**: Prompts for different writing tasks (abstract feedback, transition improvement, argument strengthening).

**Rationale**: Writing is common use case requiring nuanced guidance about appropriate boundaries.

### **Week 7: Code and data analysis assistance**

**Core content**: Using AI for code generation, debugging, and data wrangling in R, Python, and statistical software. The critical caveat: code may run without errors but produce incorrect results. Verification strategies and domain knowledge requirements.

**Exercise**: Natural language to code challenge—describe an analysis goal in plain language, generate code, execute it, and verify results against expectations. Document any corrections needed. (Non-coders: work through tutorial example; document what questions you'd need answered to verify.)

**Mid-week content**: Common debugging prompts; strategies for verifying statistical outputs.

**Rationale**: Practical skill with clear evidence base; emphasis on verification reinforces critical evaluation theme.

### **Week 8: Emerging applications—qualitative analysis and study design**

**Core content**: Experimental applications with promise and risk. AI in qualitative coding—what it can and cannot do, epistemological tensions with interpretive traditions. Using AI for study design feedback and methodology critique. Survey simulation and its contamination risks.

**Exercise**: If working with qualitative data: code a transcript excerpt manually, then with AI; compare codes and reflect on differences. If quantitative: have AI critique a study design or methodology section; evaluate the feedback quality.

**Mid-week content**: Prompt frameworks for qualitative analysis; checklist for evaluating AI methodology feedback.

**Rationale**: Positions experimental applications appropriately—interesting but requiring caution; develops judgment about application maturity.

### **Week 9: Building sustainable AI practices**

**Core content**: Avoiding over-reliance and skill atrophy, building metacognitive habits for ongoing development, creating personal AI use policies. Bias awareness and mitigation in your research context. Environmental and equity considerations.

**Exercise**: Develop personal AI use guidelines for your research—specifying where you will/won't use AI, your verification practices, and documentation standards. Create troubleshooting journal framework for ongoing reflection.

**Mid-week content**: Self-assessment tools (adapted SNAIL scale); reflection prompts for ongoing practice.

**Rationale**: Builds toward independence; creates structures for continued development beyond course.

### **Week 10: Integration, teaching, and looking forward**

**Core content**: Integrating AI across the research workflow while maintaining scholarly values. Teaching and mentoring others in responsible AI use. The evolving landscape—how to stay current without chasing every new tool. Contributing to disciplinary conversations about AI norms.

**Exercise**: Create an AI integration plan for a current or upcoming research project, specifying AI role at each stage, verification procedures, and documentation approach. Optional: develop a brief AI guidance document for students or colleagues.

**Mid-week content**: Resources for continued learning; template for AI integration planning.

**Rationale**: Culminating synthesis; positions participants as contributors to evolving norms, not just recipients of guidance.

---

## **Design principles for exercises and mid-week content**

**Exercises should use participants' own data and questions** wherever possible, with public alternatives for those without suitable materials. Recommended public datasets include the General Social Survey, American National Election Studies, Pew Research Center data, and ICPSR qualitative archives. Exercises should always include reflection components asking what worked, what didn't, and what was learned.

**Mid-week content serves multiple functions**: practical resources (checklists, templates, tool guides), connection to broader community (discussion prompts, sharing invitations), and scaffolding for the main exercises. Keep these brief—500 words maximum—and action-oriented.

**Assessment and self-assessment** should rely on portfolios documenting AI interactions and reflections, practical demonstrations of skill, and self-assessment using validated instruments (the SNAIL scale can be adapted). Avoid knowledge tests that encourage surface learning.

---

## **Key resources and further reading for course development**

The most valuable frameworks for structuring the course include the **UNESCO AI Competency Framework** (three levels across five dimensions), **Stanford Teaching Commons AI Literacy Framework** (functional, ethical, rhetorical, and pedagogical domains), and the **Digital Promise AI Literacy Framework** (understand, evaluate, use modes). For ethics specifically, COPE position statements and publisher policy summaries provide authoritative guidance.

For practical applications, the Stanford "10 Simple Rules for AI-Assisted Grant Writing" offers immediately actionable guidance. The British Journal of Educational Technology publishes ongoing research on AI in education. The Center for Open Science's AI evaluation initiatives connect to reproducibility and open science values.

The research strongly supports a course that **teaches principles over procedures, develops critical judgment alongside practical skills, and builds metacognitive habits that transfer across tools as they evolve**. The goal is not AI proficiency but AI wisdom—the judgment to know when, how, and whether to use these powerful but limited tools in service of scholarly inquiry.

# **ChatGPT report**

# Designing a 10-Week “AI for Research” Email Course

Graduate students and academic researchers are increasingly exploring **generative AI** as a tool in research. To ensure this exploration is effective and responsible, a structured learning journey can instill fundamental technical knowledge, practical skills, and ethical mindsets. Below is a comprehensive plan for a 10-week email course titled **“Getting Started with Generative AI in Research”**. This course avoids focusing on specific, transient tools; instead, it emphasizes enduring principles, skills, and reflective practices. Each week includes core concepts and a suggested hands-on exercise (using either the learner’s own research context or publicly available data) to solidify learning.

## Key Skills and Mindsets for Human–AI Collaboration in Research

Before diving into the week-by-week curriculum, it’s important to highlight the **key skills and mindsets** that successful human–AI collaboration in research entails:

* **AI Literacy – Understanding Capabilities & Limitations:** Researchers should grasp what generative AI *can and cannot do*. This means knowing AI’s strengths (e.g. pattern recognition, rapid data processing) and its weaknesses (e.g. lack of true understanding, potential for errors/bias)[\[1\]](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/#:~:text=Understanding%20what%20AI%20can%20and,AI%20can%20complement%20each%20other)[\[2\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=To%20get%20the%20most%20out,it%20creates%20and%20anticipating%20hallucinations). An AI tool may spark new ideas and handle routine tasks efficiently, but it works by recognizing patterns in training data, not by *ground truth* comprehension[\[3\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,access%20to%20web%20searches%20and). Recognizing these boundaries helps in spotting suitable use-cases for AI and avoiding misplaced trust.  
* **Effective Communication (Prompting) with AI:** Interacting with AI is an iterative, communicative process. Crafting clear, contextual prompts and instructions is key to getting useful outputs[\[4\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=3). This “prompt engineering” skill is essentially the ability to **ask good questions and give good guidance** to the AI, much like instructing a research assistant. Successful collaborators learn to refine prompts based on AI responses, guiding the AI to better results. A practical tip is to have the AI reflect on your prompt – for example, asking *“Is there anything I should clarify or ask differently?”* – which can reveal missing details and improve outcomes[\[5\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20you%20might%20also%20need,that%20it%20needs%20to%20excel).  
* **Critical Evaluation and Verification:** Perhaps the most crucial skill is **critical thinking** applied to AI outputs[\[6\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=4). Researchers must **validate facts, check sources, and scrutinize AI-generated content** just as they would human-generated work. Generative AI is notorious for “hallucinating” – producing plausible-sounding but incorrect or fabricated information. As such, any literature summaries, code, or text it generates should be cross-checked with trusted sources or ground truth data[\[2\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=To%20get%20the%20most%20out,it%20creates%20and%20anticipating%20hallucinations). Knowing when to trust AI and when human insight is needed is part of this skill[\[7\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=The%20ability%20to%20think%20critically,%E2%80%9D). In short, **the human remains responsible for the integrity and accuracy of any result**, even if an AI helped produce it[\[8\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Authorship%3A%20We%20posit%20that%20GenAI,to%20rest%20with%20the%20human).  
* **Domain Knowledge and Contextual Judgement:** AI is a powerful pattern-spotter, but it lacks contextual understanding of your specific research nuances. **Human expertise in the discipline** is needed to guide the AI (providing correct context or constraints) and to interpret the AI’s output meaningfully. Successful human–AI collaboration leverages **the researcher’s insight to ask the right questions and to recognize which AI outputs make sense** in context[\[9\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=different%20skills%20humans%20and%20AI,bring%20to%20the%20equation).  
* **Creative Thinking and Ideation with AI:** Rather than replacing human creativity, AI can augment it. Researchers skilled in collaboration use AI as a **creative partner** – for brainstorming ideas, uncovering connections, or generating multiple approaches to a problem. Importantly, they remain aware of the risk of AI biasing their creativity (e.g. AI can cause *convergence* of ideas). For instance, one study found groups using ChatGPT generated higher average-quality ideas but with far less originality (many ideas were similar) compared to groups ideating without AI[\[10\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=One%20group%20was%20told%20to,in%20the%20human%20group). Thus, maintaining one’s own independent thinking while using AI as a springboard is a valued skill.  
* **Ethical and Responsible Use:** A collaborative mindset means **using AI thoughtfully and ethically**. Researchers must be aware of issues like bias in AI outputs, privacy concerns when inputting data, plagiarism and attribution, and compliance with academic norms or policies[\[11\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,in%20the%20same%20way%20it)[\[12\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=GenAI%20offers%20new%20affordances%20that,appropriate%20attribution%20because%20current%20LLM). *Ethical AI use* involves treating AI outputs with the same rigor as any source: e.g. **citing sources for AI-assisted content, disclosing AI involvement if required, and ensuring no confidential data is exposed to public AI tools**[\[8\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Authorship%3A%20We%20posit%20that%20GenAI,to%20rest%20with%20the%20human)[\[13\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Regulations%3A%20Any%20use%20of%20GenAI,extension%20to%20implications%20for%20subsequent). An AI-literate researcher also knows how to **spot bias or problematic content** in AI outputs and mitigate it (for example, noticing if an AI’s answer reflects gender or cultural stereotypes and adjusting the prompt or output accordingly[\[14\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Potential%20for%20Bias%3A%20Just%20as,This%20may)).  
* **Continuous Learning and Adaptability:** The AI landscape evolves rapidly. Successful users adopt a **mindset of continuous learning**, staying updated on new tools, capabilities, and guidelines. They experiment with AI tools hands-on and learn from failures to improve their techniques[\[15\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=1,technology)[\[16\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20for%20this%20exploration%20to,50%2C%20and%20then%20exceeds%20that). They also stay tuned to evolving best practices (e.g. emerging journal policies on AI, new ethical guidelines) so their use of AI remains current and responsible[\[17\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=visual%20arts,progress%20for%20years%20to%20come). In essence, *AI collaboration is a skill that improves with ongoing practice and education*, much like digital literacy in earlier generations[\[18\]](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/#:~:text=What%20AI%20Literacy%20Actually%20Means).

Many academic institutions are beginning to provide resources to cultivate these skills. For example, Cornell University’s task force on AI in research urges improving “AI literacy” across the research community – helping researchers understand appropriate use, limitations, and trade-offs of generative AI tools[\[19\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=leadership,using%20such%20tools%20in%20research). Universities like Georgetown, Wisconsin, and Brown have published guides for students and faculty to *“navigate the quickly evolving terrain of generative AI,”* covering basic concepts, effective uses, and ethical considerations in academic work[\[20\]](https://www.bc.edu/content/bc-web/sites/generative-ai/resources.html#:~:text=Resources%20,evolving%20field%20of%20generative%20AI)[\[21\]](https://libguides.brown.edu/c.php?g=1338928&p=9868284#:~:text=Generative%20Artificial%20Intelligence%20,AI%20tools%20in%20academic%20work). These resources echo the above skill areas, underscoring that **using AI in research requires both technical understanding and responsible judgment**. With these core competencies in mind, we can now outline a week-by-week plan to build them.

## 10-Week Course Outline

Each week’s email will focus on a theme, combining **technical foundations** with **practical applications** and **ethical reflection**. The content is tool-agnostic – exercises can be done with any available AI platform (e.g. an open-source tool or a well-known AI assistant), and the emphasis is on principles that won’t quickly go out of date. Learners are encouraged to *“try this with your own data/ideas”* or with suggested public datasets or examples, in order to directly apply the concepts. Below is the proposed outline:

1. **Week 1: Introduction to Generative AI in Research** – This kickoff sets the stage by explaining **what generative AI is** (large language models, image generators, etc.) and **why it matters for researchers**. We’ll cover a high-level view of how generative models work (training on large datasets to learn patterns, then generating new content) and discuss the current wave of AI in academia. Importantly, this week addresses the *potential* of AI for research alongside its *limitations*. For example, generative AI can **spark new ideas by connecting prior knowledge in novel ways**[\[22\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=This%20exciting%20capability%20to%20spark,source%20approaches) and dramatically improve efficiency on certain tasks (like scanning literature or coding)[\[23\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,intensive%2C%20and%2For%20rewarding%20tasks), but it can also produce incorrect or biased outputs if not carefully checked. Real examples of AI in research are given: e.g., using an AI chatbot to brainstorm research questions, or an AI coding assistant to speed up data analysis – illustrating both the *benefits* (efficiency, scale) and *pitfalls* (errors, “black box” results)[\[24\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=output%20in%20dramatically%20less%20time%2C,sets%20that%20were%20previously%20limited)[\[11\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,in%20the%20same%20way%20it). The email also frames the course’s philosophy: AI is presented not as a magic solution, but as a **powerful tool that, in skilled hands, can augment a researcher’s capabilities**[\[9\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=different%20skills%20humans%20and%20AI,bring%20to%20the%20equation). *Exercise:* Try a simple exploration – for instance, ask a generative AI to **explain your research topic in plain language**. Observe how it performs, and note any surprising strengths or mistakes. This warm-up reinforces that AI can be handy (e.g. simplifying jargon) but also may confidently make up facts – a theme to remember throughout the course.  
2. **Week 2: Core Concepts – How Generative AI Works (No PhD in ML Required)** – In week 2, we delve into **technical foundations** at a conceptual level, providing researchers with enough understanding of the “engine under the hood” to use AI intelligently. We explain in accessible terms how models like GPT are trained (learning from vast text data to predict the next word, etc.), why they sometimes *“hallucinate”* false information, and why they might exhibit biases present in training data[\[3\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,access%20to%20web%20searches%20and)[\[14\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Potential%20for%20Bias%3A%20Just%20as,This%20may). For example, we clarify that *these models don’t “know” facts like a database – they generate text by statistical pattern-matching*, which is why a perfectly authoritative-sounding answer can be completely wrong if the pattern leads it astray[\[11\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,in%20the%20same%20way%20it). We also introduce key terms: *large language model (LLM), training data, prompt, hallucination, bias,* etc., so that participants can navigate AI discussions. Understanding these basics helps researchers appreciate limitations – e.g. *“the AI has no knowledge beyond its training data timeframe”* or *“it might reflect biases from its sources”*. Simple analogies (like *“you don’t need to build a car engine to drive, but you should know the rules of the road”*[\[25\]](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/#:~:text=What%20these%20roles%20increasingly%20require,you%E2%80%99ll%20shine%20in%20your%20field)) reinforce that researchers don’t need to be AI engineers, but should grasp how the tool operates and the “rules” for using it safely. *Exercise:* To cement these concepts, the email might include a fun mini-quiz or thought experiment – e.g., present a *dummy AI output containing a hallucinated reference* and ask the student to identify what’s suspect about it. Or encourage them to query the AI on a topic *beyond its knowledge cutoff* (for instance, a very recent event) and see how it responds. This reveals the gaps in the AI’s knowledge and reinforces the need for skepticism and understanding of the technology’s bounds.  
3. **Week 3: Communicating with AI – The Art of Prompting** – Now that the foundations are laid, week 3 hones a very practical skill: **prompt engineering**. We cover techniques for formulating questions or instructions to get useful results from generative AI. Key principles include being specific about your request, providing context or constraints, and requesting output in helpful formats (for example, *“List 3 possible hypotheses about X with supporting rationale…”*). We discuss how **iterative interaction** is often necessary – you might start with a broad prompt, get a general answer, then ask follow-up questions or refine your prompt to drill down on what you need. This iterative, conversational approach is framed as a way of “**collaborating**” with the AI, treating it like a junior research assistant that needs guidance. We also introduce the idea of **meta-prompts**: asking the AI to critique or improve its own answer. For instance, as AI experts suggest, ending a prompt with *“What else should I consider or ask you to get a better answer?”* can prompt the AI to reveal missing pieces[\[5\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20you%20might%20also%20need,that%20it%20needs%20to%20excel). Real examples are provided, such as how a poorly phrased query can lead to a useless answer, whereas a well-structured prompt yields a detailed, relevant result – this highlights the *value of clear communication*. The week’s content might cite scenarios like an AI assisting in coding: “write a Python function to do X,” and how adding details (e.g., data format or edge cases) makes the output more correct. *Exercise:* Participants are encouraged to **experiment with prompting** on a task of their choice. For example, *take a paragraph of your writing and prompt the AI to improve its clarity*, then refine the prompt to emphasize keeping the academic tone. Or, *ask the AI to suggest research questions on a topic, then try rephrasing the prompt in at least two different ways* (one vague, one specific) and compare the quality of responses. This hands-on practice will let them see how prompt changes impact AI behavior, reinforcing the lesson that **you often get what you ask for (and *how* you ask for it)**.  
4. **Week 4: Literature Review with AI – Exploring and Summarizing Scholarship** – This week focuses on using generative AI to navigate scientific literature and knowledge. The vast volume of papers and data can overwhelm researchers, and here we highlight AI’s potential as a **research assistant for literature review**. We discuss strategies like using AI tools to summarize long articles or extract key points, to generate an overview of a field, or even to discover connections between topics. For instance, generative AI can quickly provide a summary of a paper’s methodology or compare two studies’ findings if prompted correctly. We introduce a few example tools (without focusing on any one specifically) – e.g. mention that there are AI-powered literature discovery platforms (like Semantic Scholar’s AI features or Elicit) that **retrieve and synthesize information across many sources**[\[26\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=track%20of%20vastly%20more%20information,facilitating%20the%20discovery%20of%20relevant)[\[27\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=as%20Google%20Scholar%20and%20PubMed%2C,research%20across%20diverse%20academic%20disciplines). The email warns, however, about **verification and citation** issues: AI might output a convincing-sounding scientific claim or a reference that is completely fake. One suggested best practice (from current guidance) is to *use AI to summarize or suggest references, but always cross-check the original papers* – especially since LLMs can invent references that don’t exist[\[28\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=researchers%20should%20fact,rewriting%20the%20style%20of%20the)[\[29\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Duty%20of%20verification,assisted). Another tip: *provide AI with a block of text (like an abstract) and ask for a summary or critique*, rather than asking open-endedly about a field, to ground it in real data and reduce fabrications. Ethical use is emphasized: e.g., if AI helped draft a portion of a literature review, the researcher should ensure no plagiarism (perhaps by **writing the first draft in their own words, then using AI to polish**[\[30\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=comprehensiveness%20and%20accuracy%20of%20the,the%20authors%E2%80%99%20own%20work%2C%20as)). We also cover how AI might help bridge interdisciplinary gaps – finding links between concepts in different fields that a researcher might not know to connect[\[26\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=track%20of%20vastly%20more%20information,facilitating%20the%20discovery%20of%20relevant). *Exercise:* A practical task could be: *Choose a seminal paper in your field (or use a provided open-access paper). Ask an AI to summarize the paper’s key findings or to explain the paper’s significance in plain terms.* Then compare the AI’s summary to your own understanding or to the paper’s abstract. Does it miss anything or add incorrect info? Learners can also try *having the AI suggest 5 references related to a specific topic*, then verifying if those references are real and relevant. This exercise will teach them how to incorporate AI into literature review while keeping a critical eye (e.g., catching a fake citation or an implausible summary).  
5. **Week 5: Idea Generation and Study Design – AI as a Brainstorming Partner** – In week 5, the focus shifts to **research creativity and planning**. Here we explore how generative AI can assist in the **ideation phase** of research – formulating research questions, hypotheses, or even methods. For example, an AI can help by generating a list of potential research questions on a given topic, proposing imaginative hypotheses to test, or suggesting creative approaches from analogous fields. This can be especially useful for breaking out of writer’s block or when seeking interdisciplinary angles. We underscore that AI-generated ideas can be *thought-provoking*: one researcher described ChatGPT as *“an enormous opportunity to improve… and get access to a lot of fairly reliable raw material”* for developing better questions[\[31\]](https://www.frontiersin.org/journals/research-metrics-and-analytics/articles/10.3389/frma.2024.1486832/full#:~:text=). The AI, in effect, can act like a brainstorming buddy that *doesn’t tire of tossing out ideas*. However, we caution that **originality is key** – AI might generate very conventional ideas (because it’s drawing from common patterns in existing literature). To ensure uniqueness, researchers should use the AI’s suggestions as a *starting point*, then apply their own insight and twists. We also show how AI can contribute to **study design**: for example, drafting sample survey questions, suggesting how to operationalize a concept, or generating possible experimental setups. Indeed, AI can even help create small pieces of a proposal (say, listing variables that might affect an outcome, or generating an illustrative example scenario for a study). By automating some grunt work, the researcher is “freed to focus more on the ideas,” as one academic noted[\[32\]](https://www.frontiersin.org/journals/research-metrics-and-analytics/articles/10.3389/frma.2024.1486832/full#:~:text=Zhu%20said%20that%20ChatGPT%20had,%E2%80%9D). Yet, integrity comes first – any design must be evaluated by the researcher for feasibility and ethical soundness. We also address that using AI in ideation should not make one complacent: *the goal is to enhance human creativity, not stifle it*. (Recall the finding that heavy AI involvement can cause idea convergence[\[10\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=One%20group%20was%20told%20to,in%20the%20human%20group); one should consciously seek diverse perspectives beyond what the AI easily provides.) *Exercise:* Learners are prompted to *use AI for brainstorming* their research topic. For instance: “Ask the AI to suggest three possible research questions you could pursue related to your thesis topic (or a public dataset/problem provided),” or “Have the AI propose imaginative extensions or applications of a theory you’re interested in.” Then, the key step: *evaluate those suggestions*. Which ideas are novel or useful? Which seem dubious or too generic? Participants can then refine one of the AI’s ideas with their own expertise – essentially *collaborating* with the AI to improve an idea. This exercise demonstrates how human insight and AI output can combine, and it reinforces the researcher’s role in guiding the creativity process.  
6. **Week 6: Data Analysis and Coding Assistance with AI** – Week 6 gets into the nitty-gritty of research execution: using AI to help analyze data or perform technical tasks. For researchers in social and behavioral sciences (our focus area), this could include both **quantitative and qualitative** assistance. On the quantitative side, we show how AI coding assistants (like GitHub Copilot or GPT-4’s code generation abilities) can write snippets of code for data cleaning, statistical analysis, or visualization[\[33\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=G%20enAI%20for%20Research%20Infrastructure)[\[34\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=software%2C%20using%20complicated%20APIs%20,APIs%20for%20generating). For example, instead of combing StackOverflow for how to run a particular test in R or Python, one can prompt the AI: *“Help me write code to perform a thematic analysis of text data”* or *“Plot the distribution of variable X with labels”*. The AI often produces a workable starting script in seconds[\[34\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=software%2C%20using%20complicated%20APIs%20,APIs%20for%20generating). This can **accelerate the workflow dramatically**, especially for those with limited programming experience – turning some of the coding into a dialogue with an assistant. On the qualitative side, we discuss using AI to summarize or code qualitative data. For instance, feeding interview transcripts (carefully, respecting privacy\!) to an AI and asking for summary of main themes, or even having it suggest possible codes or categories. Another example: using AI to critique a draft survey or suggest additional interview questions (leveraging its vast knowledge to point out what you might miss). Throughout, a **“duty of verification”** is stressed[\[29\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Duty%20of%20verification,assisted): if AI writes code, the researcher must test and debug it; if AI analyzes data, the researcher must confirm the results with proper validation. There have been cases where AI-written code *looks* correct but has subtle errors, or where AI’s statistical answer is plainly wrong because it lacks true numerical understanding. We encourage treating AI as an “intern” – helpful and quick, but requiring oversight. We also caution about data privacy: never paste sensitive or proprietary data into a public AI service without clearance[\[13\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Regulations%3A%20Any%20use%20of%20GenAI,extension%20to%20implications%20for%20subsequent). If possible, use local or institution-approved tools for analysis. *Exercise:* A hands-on idea: using a provided public dataset (or one from the student’s research if available), ask the AI to perform a simple analysis. For example, *provide summary statistics or identify any trends in the data*. If coding, they could use an AI to generate code for a task (like performing a linear regression or creating a chart). The student then runs that code (or examines the reasoning) to see if it works and makes sense. If the code fails or the summary is off, that’s actually a valuable lesson – they can iterate by telling the AI the error or confusion and seeing how it debugs. By doing this, participants learn how AI can be a coding co-pilot or analysis helper, and also **learn the importance of testing AI outputs**. They might end up with a useful script or a summary, but more importantly, they gain practice in **supervising AI’s technical contributions**.  
7. **Week 7: Writing and Publication – AI as a Writing Assistant** – In academic research, writing is a major component – from papers and proposals to presentations. This week examines how generative AI can assist in **academic writing tasks**. We discuss using AI for tasks like: improving grammar and clarity in a draft, suggesting alternative phrasings, summarizing a long section into an abstract, or even **translating text between technical and layman versions**. A noted benefit of AI writing assistance is helping non-native English speakers by leveling the linguistic playing field – AI can suggest more fluent wording and fix language issues, helping the author express their ideas more clearly[\[12\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=GenAI%20offers%20new%20affordances%20that,appropriate%20attribution%20because%20current%20LLM). The course module, however, makes a firm distinction: *AI is a tool for editing and refining your own ideas, not a ghostwriter to generate content you don’t understand*. We echo emerging norms (e.g. many journals’ policies) that **authors are responsible for the content** – if an AI writes a paragraph, the researcher must verify every fact and ensure it reflects *their* interpretation[\[8\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Authorship%3A%20We%20posit%20that%20GenAI,to%20rest%20with%20the%20human). We cover best practices such as: start by writing a rough draft or bullet points yourself, then use AI to polish or expand it. Or use AI to **generate a first draft for mundane sections** like boilerplate text (e.g. a generic methods description), but then *heavily edit it to fit your specific work and check for accuracy*. We address the risk of plagiarism and loss of originality – for instance, if an AI pulls a common phrasing from literature, the author might inadvertently use it without citation. To avoid this, a tip from Week 4 is reinforced: *write first, then let AI refine*, so the core content is yours[\[35\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=work%20but%20provide%20incorrect%20or,for%20a%20summary%20of%20existing). Additionally, we mention the need to possibly **acknowledge AI assistance** in writing if required by a venue (some journals require disclosure if AI was used for editing or writing). On the positive side, AI can help overcome writer’s block (e.g. *“suggest a way to start this introduction”*) and even act as a pseudo-*peer reviewer* by critically assessing a draft you feed it (though we caution not to share sensitive drafts with public tools). We also touch on using AI to generate visual aids: e.g. creating images or diagrams for papers or presentations (with proper attribution and caution about data visualization accuracy). *Exercise:* This week, participants can pick a piece of their academic writing (perhaps a paragraph from a paper or a thesis chapter, or use a sample text provided) and use a generative AI to **edit or improve it**. For example, *ask the AI to rewrite the paragraph for clarity and conciseness*. Then the student should compare the edited version to the original: Is the meaning preserved? Is anything inaccurate introduced? They can also prompt the AI to *format text in a certain style (APA style references, for example)* or *generate a short summary of their text*. By doing this, they see firsthand how AI can act as an “editor”. Another possible exercise: have the AI *suggest a title or create a brief press-release-style summary* of one of their papers – illustrating how AI might help in communicating research to broader audiences. The main outcome is learning to use AI as a writing aid while **keeping scholarly control and voice**.  
8. **Week 8: Ethics and Responsible AI Use in Research** – The dedicated ethics week encourages reflection on the broader implications of integrating AI into research. By now, learners have tried various applications; this module prompts them to step back and consider guidelines and their **“duty of care”** when using AI. Key ethical topics include: **plagiarism and academic integrity** (e.g., it’s unacceptable to have AI write whole papers for you – aside from violating integrity, you might propagate errors or commit undisclosed ghostwriting, which many consider misconduct[\[36\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Following%20from%20the%20definition%20of,the%20output%20that%20is%20produced)[\[8\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Authorship%3A%20We%20posit%20that%20GenAI,to%20rest%20with%20the%20human)); **bias and fairness** (AI models often encode biases present in their training data, so one must be vigilant – e.g. AI might generate stereotypical content, as in an example where an AI-generated hospital scene had all doctors as male[\[14\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Potential%20for%20Bias%3A%20Just%20as,This%20may); researchers should be aware and correct such biases in AI outputs); **data privacy** (discuss why inputting raw research data or sensitive information into cloud AI services can breach confidentiality or data protection rules[\[13\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Regulations%3A%20Any%20use%20of%20GenAI,extension%20to%20implications%20for%20subsequent) – always check institutional policies, and prefer approved tools for sensitive data); **transparency and disclosure** (encourage researchers to be transparent about if and how AI was used in their process, especially in publications – this is becoming part of *research integrity* to disclose significant AI contributions to analysis or writing[\[37\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Impact%20on%20Concepts%20and%20Interpretations%3A,draft%20a%20related%20work%20section)); and **reproducibility** (AI tools can change over time or produce non-deterministic results – how do we ensure our AI-assisted methods are reproducible? Suggestions include documenting AI steps, saving prompt-output pairs, etc.). We likely reference guidelines from institutions: for example, Ohio State’s principle of *applying the same standards to AI-assisted work as to any other work, balancing AI’s efficiency with the responsibility to review and verify everything for accuracy and bias*[\[38\]](https://omc.osu.edu/expertise-areas/generative-ai#:~:text=Whether%20gathering%20information%2C%20streamlining%20tasks%2C,accuracy%2C%20tone%20and%20audience%20impact)[\[39\]](https://omc.osu.edu/expertise-areas/generative-ai#:~:text=,incorrect%2C%20misleading%20or%20biased%20results). We also stress that the **human researcher is ultimately accountable** for any output – AI is an extension of your toolset, not an excuse for carelessness[\[8\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Authorship%3A%20We%20posit%20that%20GenAI,to%20rest%20with%20the%20human). Another angle: discuss the ethical implications for the research community – if some use AI heavily, does that create unfair advantages, or challenges in peer review? The course encourages *responsible leadership* – e.g. if these participants supervise students or collaborate, they should share ethical norms and not assume everyone knows them[\[40\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=AI%20Literacy%20to%20support%20Research,authorship%2C%20privacy%20regulations). *Exercise:* This week’s task is more reflective. Learners can perform an *“AI audit”* on one of their own small projects or on a provided scenario. For instance: *Write down ways in which using AI could introduce ethical issues in a hypothetical study (like bias in choosing literature, or privacy in using data, or misattribution in writing). Then outline steps to mitigate each issue.* Alternatively, they could be given a short AI-generated blurb and asked to identify any ethical red flags (e.g., does it cite a source? could any part be plagiarized? is any language biased or inappropriate?). By articulating these considerations, they solidify an ethical framework for AI use. The email might also include a short checklist for ethical AI use in research as a takeaway reference (for example: “Always fact-check AI outputs; Never input confidential data into unapproved tools; Disclose AI contributions in publications; etc.”).  
9. **Week 9: Human–AI Collaboration Best Practices and Evolving Workflows** – In week 9, the focus is on putting it all together: **developing a personal workflow that productively integrates AI into research**. We shift from individual tasks to the *meta-level*: how do you, as a researcher, collaborate with AI through your project lifecycle? We provide best practices gathered from earlier weeks and external examples. One concept to emphasize is **“AI as a partner, not a replacement.”** Research from industry notes that humans \+ AI together can achieve outcomes neither could alone[\[9\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=different%20skills%20humans%20and%20AI,bring%20to%20the%20equation), and the “magic” lies in partnership where each party does what it’s best at[\[41\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=Collaboration%20is%20the%20key%20to,success). For example, AI can churn through data or text quickly, while the human provides critical interpretation and ethical oversight[\[42\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=AI%20excels%20at%20pattern%20recognition%2C,%E2%80%9D). We outline a scenario of an AI-augmented research workflow: starting from idea generation (AI helps brainstorm, human refines), to literature review (AI summarizes, human analyzes credibility), to experiment design (AI suggests variations, human judges feasibility), to analysis (AI writes draft code, human validates results), to writing (AI helps edit, human ensures clarity and truth). This narrative shows how AI can slot into many research stages, each time requiring the researcher’s guidance (a concept Cornell’s framework also reflects in the “four stages of research” and corresponding *duties* of the researcher at each stage[\[43\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=These%20four%20stages%20that%20can,life%20cycle%20of%20research%20include)[\[29\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Duty%20of%20verification,assisted)). We provide **practical collaboration tips**: for instance, set aside time to “play” with AI on your project (echoing the idea that experimentation is key to mastery[\[15\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=1,technology)), but also set boundaries (know when *not* to use AI – e.g., when originality of thought is paramount, or when interpreting nuanced qualitative nuances that AI might miss). Another tip: maintain a log of how AI was used (prompts and outcomes), which helps in both transparency and reflecting on what worked or not. We also address the emotional aspect – some researchers fear AI could make them obsolete or weaken their skills. On the contrary, we frame that **developing AI collaboration skills will be increasingly expected** and valued, as studies show jobs requiring AI skills are growing and often higher-paid[\[44\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20it%20isn%E2%80%99t%20just%20companies,from%20last%20year). The point is to “work smarter” by offloading rote tasks to AI and focusing human effort on high-level thinking. We might share a short anecdote: e.g., a researcher who treated an AI agent as a *team member* to automate email replies overnight, and then simply reviewed and sent them in the morning – saving hours[\[45\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=Niles,adopt%20her%20tone%20and%20voice)[\[46\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=could%20manage%20her%20inbox,adopt%20her%20tone%20and%20voice). This illustrates trust-building: the researcher didn’t blindly trust the AI, but through oversight and gradual use, they built confidence and achieved efficiency. *Exercise:* Learners are encouraged to draft a **personal plan or policy for human–AI collaboration** in their work. For example: *Outline which research tasks you will use AI for and how, versus tasks you will deliberately do manually. How will you ensure quality control?* This might take the form of a short workflow diagram or checklist they create for themselves (and perhaps share with peers if this course had a forum). Another activity: *Revisit a past research project you did and identify points where an AI tool could have been helpful. How would you incorporate it? Would it change your results or confidence?* This retrospective exercise helps in visualizing integration of AI into future projects. By consciously planning the collaboration, researchers can optimize their workflow while upholding integrity.  
10. **Week 10: Reflection, Future Trends, and Continuing Your AI Journey** – The final week serves as both a conclusion and a look ahead. We prompt participants to **reflect on their learning**: What new skills have they developed? How do they plan to apply generative AI in their upcoming research projects? This recap reinforces the progress from week 1 (perhaps they recall how naive or skeptical they were) to now being more AI-literate and confident, yet also *more critically aware*. We encourage a forward-looking mindset: generative AI technology will continue to evolve (new models, new capabilities, changes in what AI can do). To avoid this course from ever becoming stale, we emphasize **principles for staying up-to-date**. Suggestions include: following relevant research blogs or academic forums on AI, joining communities of practice (for instance, an online group for scientists using AI in research, or a local university working group). Many institutions are actively updating guidelines – staying informed on those will be part of one’s professional development[\[17\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=visual%20arts,progress%20for%20years%20to%20come). We also mention *future trends* in generative AI that could impact research, such as multimodal AI (handling text, data, images together), AI tools specialized for academic research (maybe open-source models trained on academic knowledge), or improved citation and fact-checking features in AI (to combat the hallucination problem). The idea is not to teach these in detail, but to make learners aware that the field is dynamic and they should maintain a learner’s attitude. We circle back to the fundamental mindsets: **continuous learning, adaptability, and ethical leadership**. As one university’s guidance put it, *“embrace continuous learning and collaboration”* in AI use[\[47\]](https://omc.osu.edu/expertise-areas/generative-ai#:~:text=3%20We%20embrace%20continuous%20learning,and%20discovery) – meaning researchers should keep experimenting, sharing experiences with colleagues, and collectively developing best practices as AI advances. Another future-oriented point: consider how AI might change the culture of research (for instance, routine writing might be faster, but critical thinking and creativity will become even more the differentiators). We encourage participants to be on the leading edge of using these tools **responsibly to advance knowledge**, rather than fearing them or using them recklessly. *Exercise:* The course finale could ask participants to *write a short “AI usage manifesto” or a set of resolutions* for themselves going forward. For example: *“I will use AI to expedite tedious tasks, but I will always maintain responsibility for my work. I will continue to improve my prompting skills and stay informed about new AI tools in my field. I will mentor others in my lab on ethical AI use, etc.”* This personal commitment solidifies what they’ve learned. Additionally, we might invite them to imagine one exciting way AI could transform their field in the next 5-10 years, and one potential challenge to watch out for – reinforcing that they, as emerging scholars, have a role in shaping how AI is adopted in research.

## Conclusion and Additional Resources

By the end of this 10-week journey, researchers should feel equipped with a **strong foundation in using generative AI as a powerful extension of their research toolkit**. They will have learned not just *how* to use various AI capabilities (from literature search to writing), but more importantly *when and when not to use them*, and *how to do so ethically and effectively*. The emphasis on exercises like “try this on your own data” ensures that skills are applied to real-world contexts, making the learning immediately relevant.

To support continued growth, the final email can include a curated list of resources for further reading and community support, for example:

·  	**Guidelines and Reports:** The Cornell Generative AI in Academic Research report (2023) – for detailed discussion of policies and use-cases[\[48\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Generative%20Artificial%20Intelligence%20,their%20explicit%20awareness%20or%20consent)[\[40\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=AI%20Literacy%20to%20support%20Research,authorship%2C%20privacy%20regulations); various university library guides on generative AI (Georgetown, Brown, etc.) which provide tool listings and tips; and the latest publications on AI in academia (to stay aware of new ethical debates and capabilities).

·  	**Communities of Practice:** Links to forums or groups (like the [AI in Research subreddits](https://www.reddit.com/r/AcademicPsychology/) or discipline-specific AI workshops) where researchers share experiences.

·  	**Learning Platforms:** Suggestions like Coursera or university mini-courses on AI literacy, or vendor tutorials (OpenAI, etc.), especially if they release new features (ensuring the learner knows where to find *ongoing* training).

·  	**Key Reminders (Quick-Ref Guide):** A one-page summary of “Do’s and Don’ts” derived from the course, e.g. *Do fact-check, Do experiment, Don’t input sensitive data in public AI, Don’t treat AI output as truth without verification*, etc., as a handy reference.

By focusing on **fundamental skills and mindsets**, this email course remains relevant despite the fast-changing AI landscape. The goal is that participants come away not only with *knowledge* of generative AI applications, but with a reflective, adaptive approach to any new AI tool they encounter. In essence, they become confident, ethical **AI-augmented researchers** – leveraging the best of what machines can do while exemplifying the critical thinking and creativity that humans uniquely bring to research[\[7\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=The%20ability%20to%20think%20critically,%E2%80%9D)[\[49\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Impact%20on%20Methodology%3A%20Writing%20and,instrument%20that%20dulls%20them%20is). This synergy of human insight and AI capability can empower them to push the frontiers of knowledge, responsibly and innovatively.

---

[\[1\]](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/#:~:text=Understanding%20what%20AI%20can%20and,AI%20can%20complement%20each%20other) [\[18\]](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/#:~:text=What%20AI%20Literacy%20Actually%20Means) [\[25\]](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/#:~:text=What%20these%20roles%20increasingly%20require,you%E2%80%99ll%20shine%20in%20your%20field) Why AI Literacy Is Becoming as Important as Digital Literacy for Every Career Path | Pfeiffer University

[https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/](https://www.pfeiffer.edu/why-ai-literacy-is-becoming-as-important-as-digital-literacy-for-every-career-path/)

[\[2\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=To%20get%20the%20most%20out,it%20creates%20and%20anticipating%20hallucinations) [\[4\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=3) [\[5\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20you%20might%20also%20need,that%20it%20needs%20to%20excel) [\[6\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=4) [\[7\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=The%20ability%20to%20think%20critically,%E2%80%9D) [\[9\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=different%20skills%20humans%20and%20AI,bring%20to%20the%20equation) [\[10\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=One%20group%20was%20told%20to,in%20the%20human%20group) [\[15\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=1,technology) [\[16\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20for%20this%20exploration%20to,50%2C%20and%20then%20exceeds%20that) [\[41\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=Collaboration%20is%20the%20key%20to,success) [\[42\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=AI%20excels%20at%20pattern%20recognition%2C,%E2%80%9D) [\[44\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=But%20it%20isn%E2%80%99t%20just%20companies,from%20last%20year) [\[45\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=Niles,adopt%20her%20tone%20and%20voice) [\[46\]](https://www.salesforce.com/ap/blog/human-ai-collaboration/#:~:text=could%20manage%20her%20inbox,adopt%20her%20tone%20and%20voice) Human-AI Collaboration Skills Key to the Future of Work \- Salesforce

[https://www.salesforce.com/ap/blog/human-ai-collaboration/](https://www.salesforce.com/ap/blog/human-ai-collaboration/)

[\[3\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,access%20to%20web%20searches%20and) [\[8\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Authorship%3A%20We%20posit%20that%20GenAI,to%20rest%20with%20the%20human) [\[11\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,in%20the%20same%20way%20it) [\[12\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=GenAI%20offers%20new%20affordances%20that,appropriate%20attribution%20because%20current%20LLM) [\[13\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Regulations%3A%20Any%20use%20of%20GenAI,extension%20to%20implications%20for%20subsequent) [\[14\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Potential%20for%20Bias%3A%20Just%20as,This%20may) [\[17\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=visual%20arts,progress%20for%20years%20to%20come) [\[19\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=leadership,using%20such%20tools%20in%20research) [\[22\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=This%20exciting%20capability%20to%20spark,source%20approaches) [\[23\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=,intensive%2C%20and%2For%20rewarding%20tasks) [\[24\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=output%20in%20dramatically%20less%20time%2C,sets%20that%20were%20previously%20limited) [\[26\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=track%20of%20vastly%20more%20information,facilitating%20the%20discovery%20of%20relevant) [\[27\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=as%20Google%20Scholar%20and%20PubMed%2C,research%20across%20diverse%20academic%20disciplines) [\[28\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=researchers%20should%20fact,rewriting%20the%20style%20of%20the) [\[29\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Duty%20of%20verification,assisted) [\[30\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=comprehensiveness%20and%20accuracy%20of%20the,the%20authors%E2%80%99%20own%20work%2C%20as) [\[33\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=G%20enAI%20for%20Research%20Infrastructure) [\[34\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=software%2C%20using%20complicated%20APIs%20,APIs%20for%20generating) [\[35\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=work%20but%20provide%20incorrect%20or,for%20a%20summary%20of%20existing) [\[36\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Following%20from%20the%20definition%20of,the%20output%20that%20is%20produced) [\[37\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Impact%20on%20Concepts%20and%20Interpretations%3A,draft%20a%20related%20work%20section) [\[40\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=AI%20Literacy%20to%20support%20Research,authorship%2C%20privacy%20regulations) [\[43\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=These%20four%20stages%20that%20can,life%20cycle%20of%20research%20include) [\[48\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Generative%20Artificial%20Intelligence%20,their%20explicit%20awareness%20or%20consent) [\[49\]](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/#:~:text=Impact%20on%20Methodology%3A%20Writing%20and,instrument%20that%20dulls%20them%20is) Generative AI in Academic Research: Perspectives and Cultural Norms \- Cornell Research & Innovation

[https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/](https://www.research-and-innovation.cornell.edu/generative-ai-in-academic-research/)

[\[20\]](https://www.bc.edu/content/bc-web/sites/generative-ai/resources.html#:~:text=Resources%20,evolving%20field%20of%20generative%20AI) Resources \- Generative AI \- Boston College

[https://www.bc.edu/content/bc-web/sites/generative-ai/resources.html](https://www.bc.edu/content/bc-web/sites/generative-ai/resources.html)

[\[21\]](https://libguides.brown.edu/c.php?g=1338928&p=9868284#:~:text=Generative%20Artificial%20Intelligence%20,AI%20tools%20in%20academic%20work) Generative Artificial Intelligence \- Library Guides at Brown University

[https://libguides.brown.edu/c.php?g=1338928\&p=9868284](https://libguides.brown.edu/c.php?g=1338928&p=9868284)

[\[31\]](https://www.frontiersin.org/journals/research-metrics-and-analytics/articles/10.3389/frma.2024.1486832/full#:~:text=) [\[32\]](https://www.frontiersin.org/journals/research-metrics-and-analytics/articles/10.3389/frma.2024.1486832/full#:~:text=Zhu%20said%20that%20ChatGPT%20had,%E2%80%9D) Frontiers | Global insights: ChatGPT's influence on academic and research writing, creativity, and plagiarism policies

[https://www.frontiersin.org/journals/research-metrics-and-analytics/articles/10.3389/frma.2024.1486832/full](https://www.frontiersin.org/journals/research-metrics-and-analytics/articles/10.3389/frma.2024.1486832/full)

[\[38\]](https://omc.osu.edu/expertise-areas/generative-ai#:~:text=Whether%20gathering%20information%2C%20streamlining%20tasks%2C,accuracy%2C%20tone%20and%20audience%20impact) [\[39\]](https://omc.osu.edu/expertise-areas/generative-ai#:~:text=,incorrect%2C%20misleading%20or%20biased%20results) [\[47\]](https://omc.osu.edu/expertise-areas/generative-ai#:~:text=3%20We%20embrace%20continuous%20learning,and%20discovery) | The Ohio State University

[https://omc.osu.edu/expertise-areas/generative-ai](https://omc.osu.edu/expertise-areas/generative-ai)

# **Plan**

# **Learning objectives**

* Effective interaction with GenAI \- co-intelligence, planning from the start, experimentation  
* Critical interaction \- understanding risks (hallucination, bias), transparency, choices, and where indiviuals and humans want to retain control and add value  
* Use beyond simple next-token prediction \- understanding thinking models, RAG & search grounding, agentic use, to avoid simplistic understanding and limitation claims

## **Course intent**

Participants will learn to:

1. **Interact effectively with GenAI (co-intelligence)**  
     
   * capability-aware planning from the start  
   * iterative exploration (multi-turn collaboration)  
   * prompt design as specification (constraints, roles, examples)

   

2. **Interact critically (epistemic vigilance)**  
     
   * understand hallucination, sycophancy, bias, and confidence miscalibration  
   * know where humans must retain judgment and control  
   * practice transparency and responsible disclosure

   

3. **Understand GenAI beyond simplistic “next-token only” claims**  
     
   * thinking / extended reasoning modes: what they help with, what they don’t  
   * retrieval/search grounding (RAG) and its limits  
   * agentic workflows and APIs as *intensifiers* of both benefits and risks

# **Foundational understanding**

- Key concepts: LLM, training data (knowledge cut-off, bias), prompt, chain-of-thought  
- Next word prediction engine \- *probabilistic* re-generation of average language. Do not always take the most likely word, but a likely one (this can be tuned through “temperature” setting to balance accuracy/predictability and creativity)  
- Cannot internally look up facts, but link words. So unique combinations of many words are a particular problem, such as complete academic references.  
- "Stochastic Parrot" metaphor (Bender et al.) vs "emergent reasoning"  
- AI can be used to generate text based on a short prompt \- or to transform information (e.g. from PDFs).  
- Difference in cost between generation and verification \- GenAI is great where generation is costly and verification easy (e.g. illustrations, code)  
  - Search-enabled LLMs have become a lot better at verification  
- Difference between open & closed models, local & cloud models

# **Effective interaction**

- Risks of sycophancy and hallucinations  
  - GenAI trained to give answers human raters like (reinforcement learning) \- in one-off interactions, this can come down to uncritical praise and confident lying  
  - Models have become better \- yet this also requires critical engagement with outputs and adversarial prompting  
- "hermeneutic of suspicion" / “nullius in verba” / "Epistemic Vigilance" \- not AI specific, but particularly important  
- “Prompt engineering”  
  - Many technical tips no longer necessary for top models \- LLMs trained to understand intent  
    - But can help users to clarify intent  
    - And specifying expectations helps \- though broad exploration has its value, so consider interaction rather than “one-shot”  
  - Specifying roles helps to determine who you interact with (harsh reviewer, creative sparring partner), and providing examples (few-shot prompting) helps to clarify intent and set output format  
  - Try different prompts, ask models & save key prompts useful for you  
- Different models have different focus \- ensemble of experts (within and across)

# **AI and creativity**

- Engagement with “AI” can increase the quality of individual ideas \- but leads to convergence across ideas [https://knowledge.wharton.upenn.edu/article/does-ai-limit-our-creativity/](https://knowledge.wharton.upenn.edu/article/does-ai-limit-our-creativity/) \[though each AI might well be different\]  
  - “Thinking” pushes this further

# **Effective interaction**

- Publisher / Scholarly Guidelines  
  - GenAI cannot be a co-author \- not a producer of original work. Responsibility clearly lies with user.   
  - Attribution can be a challenge \- training breaks clear link between author and ideas (though RAG-like tools can improve this)  
- AI is interdisciplinary \- boon and curse

# **Ethical considerations**

- Privacy  
  - AI is software \- each tool & provider you share data with needs to be assessed  
  - Institutions and individuals can run models on their own servers/computers \- then control data. Can use free services \- then usually the user is the product. And much in between.  
- Policies  
  - University and publishers are creating them \- make sure to check which apply to you. Worth keeping an “audit trail” where practical, e.g. by working with “projects”  
- Resource use  
  - Water & energy usage often cited as concerning \- yet digital is efficient  
  - But: no need to bring tank to a wrestling match, using smaller models make sense  
- Overall: APA ethics principles (beneficence, integrity, justice)

# **Overarching Risks**

- Not covered in detail, but as suggestions for further exploration  
  - Deskilling/skill atrophy & resulting system failures (cf aviation)  
  - Model collapse (when AI is trained on AI-generated content across the internet, becoming ever more homogeneous)  
  - Centralisation, commercialisation and ineuqality \- vs narrowing gaps, inclusivity and growth in openness  
  - Fraud & slop in the literature (parallels to earlier inventions that made knowledge creation & dissemination easier?)  
  - AGI & existential risks

# **Research use**

- Qualitative text analysis (e.g., enabling use of text data at scale, improving on text-mining)  
- Experimental design, e.g. vignettes  
- Data collection \- AI driven interviews  
- Survey data simulation and its risks

# **Learning**

- New tools all the time. Paradigm shifts relatively rarely \- transformers, chat, thinking, agents. How to tell apart?  
- How to build community, and collective reflection? Risks of silent adoption, so let’s avoid that.

# **Researching AI and consuming AI research**

- Delay challenges \- “AI can’t do x” quickly of historical interest only  
- Comparison problems \- zero bias vs human bias

# **Activities**

- Start  
  - Document current use, usefulness, concerns, questions (+ goals for the course)  
- Test 2-3 LLM chat interfaces on topics you are familiar with:  
  - Explain a concept in plain language  
  - Recommend key readings about general phenomenon / specific topic  
  - Generate or evaluate research questions/hypotheses  
    - Engage in multi-turn conversations to see how you can steer the models  
    - Evaluate the answers. What do you find helpful? What errors/problems do you spot?  
- Work with a grounded tool (e.g. NotebookLM) on a set of \~10 papers relevant to a specific project and test various types of summaries/interactions  
- Search for a topic on Google Scholar (non-AI mode) as well as in an LLM, and compare. What sources are shown?  
  - Compare LLM response, Wikipedia entry and review paper conclusion on topic you knpw. How do you judge nuance, balance, confidence?  
- Prompting:  
  - Experiment with different levels of specificity, success criteria, iteration  
  - E.g. on improving a piece of your writing  
- Coding:  
  - Get something done  
  - Understand how to do something  
  - Get feedback on your code (bugs and performance)  
  - Relevance of test-driven development  
- Agents:  
  - Use a coding agent for   
    - coding & testing  
    - exploratory data analysis  
    - confirmatory data analysis based on a pre-registration  
    - a non-coding agentic task  
- API use and text analysis  
  - Set up an API, e.g. Gemini through AI Studio  
  - Use it to extract structured responses  
- Use in research  
  - Text analysis  
    - Interactively with chat interfaces \- e.g. to develop codebooks  
    - Passively with agents (including annotation)  
    - Passively with API calls (getting summaries)  
  - Experimental design  
    - Ask to critique methodology  
    - Review materials  
    - Generate materials (e.g. for stimulus sampling)  
  - Survey data simulation (agents)  
  - Socratic vs adversarial prompting to improve research ideas  
- AI and writing  
  - Reflect:   
    - What is hard for you?  
    - Where do you benefit from doing the writing? When do ideas happen?  
    - What is your value-add? How important is writing itself in your field?  
  - Experiment:  
    - Pick a writing project that needs attention \- or that would be good to do (e.g. a blog post)  
    - Try to spot the composite voice problem \- and see whether role prompts or writing samples (or meta-prompts created from writing samples) can improve  
- Spotting bias  
  - Try to reproduce one of the many bias claims?  
- End-to-end planning (consider AI-first mindset)  
  - Pick a plan for a research project \- if you haven’t written it down clear, consider testing whether an LLM can help you elucidate it  
  - Plan which steps can outsourced to AI, done collaboratively, supported by AI vs done by you \- both from cognitive safety (centaur-cyborg-automation) and jagged frontier/capability perspective  
  - Where you are not sure, consider how you can test it  
  - Choose tools  
- AI manifesto: green zones (e.g. will not submit without asking AI to check for errors), red zone (e.g. will not let AI write first draft of discussion section) \- and guidance, e.g. verification strategies, for areas in between  
- Review AI disclosure statement in your field, write disclosure statements  
- Staying up to date  
  - Find a few people you want to follow \- e.g. Ethan Mollick  
  - Understanding jagged frontier and its shape  
  - AI in research training/supervision (need to learn writing and coding by doing it yourself?)  
  - Consider setting aside some time for experimentation  
- Use AI in peer review:  
  - On your own paper  
  - On a published paper you know  
  - Experiment with generic prompt, providing journal guidelines, and providing specific sub-questions  
    - What did the AI spot? What did the AI get wrong?  
  - Guidelines on using AI in peer review:  
    - Focus on self-review  
    - Adhere to journal policies  
    - Consider: even if AI makes each review better, it could make two reviews converge too much.

# **Weeks**

Here is the course content condensed into your requested format:

## **ChatGPT**

* **Week 1: Introduction to Generative AI in Research.** This session introduces AI as a powerful tool to augment researcher capabilities while highlighting the critical need to verify outputs for bias and inaccuracies.  
* **Week 2: Core Concepts – How Generative AI Works.** We explore the mechanics of Large Language Models (LLMs) to explain why they prioritize statistical patterns over factual databases, leading to "hallucinations."  
* **Week 3: Communicating with AI – The Art of Prompting.** Learners master prompt engineering by using specificity, context, and iterative questioning to treat the AI as a capable junior research assistant.  
* **Week 4: Literature Review with AI.** This week demonstrates how to use AI for summarizing papers and discovering connections across fields while emphasizing the necessity of cross-checking citations against original sources.  
* **Week 5: Idea Generation and Study Design.** We focus on using AI as a tireless brainstorming partner to generate hypotheses and survey questions, using human insight to refine generic outputs into novel research.  
* **Week 6: Data Analysis and Coding Assistance.** Participants learn to use AI "co-pilots" to write data-cleaning scripts and summarize qualitative themes, provided all code and results undergo strict human validation.  
* **Week 7: Writing and Publication.** AI is framed as an editorial aid for polishing clarity and overcoming writer’s block, rather than a ghostwriter, ensuring the researcher remains the sole author of the ideas.  
* **Week 8: Ethics and Responsible AI Use.** This module covers the "duty of care" regarding data privacy, institutional compliance, and the transparency required when disclosing AI’s role in scholarly work.  
* **Week 9: Human–AI Collaboration Best Practices.** We synthesize previous lessons into a cohesive workflow where AI handles high-volume rote tasks so the researcher can focus on high-level critical interpretation.  
* **Week 10: Reflection and Future Trends.** The course concludes by preparing researchers for a dynamic future of multimodal AI tools and specialized academic models through a commitment to continuous learning.

## **Claude**

* **Week 1: Foundations of Human-AI Collaboration.** This kickoff covers the technical mechanics of large language models and establishes a personal framework for the planning-monitoring-reflecting cycle.  
* **Week 2: Critical Evaluation as Core Competency.** We explore why AI generates "confident errors" and fabricated citations, emphasizing a "hermeneutic of suspicion" when verifying all outputs.  
* **Week 3: Prompt Engineering as Communication Skill.** This week reframes prompting as a transferable skill in articulating goals and decomposing tasks using structured frameworks like CLEAR.  
* **Week 4: AI for Literature Discovery and Synthesis.** Participants learn to integrate AI discovery tools into systematic workflows while maintaining the documentation required for methodological transparency.  
* **Week 5: Ethics, Transparency, and Professional Norms.** We examine publisher policies, the prohibition of AI authorship, and the application of APA ethics principles to AI-assisted research.  
* **Week 6: AI for Academic Writing.** This session distinguishes between appropriate editorial support, such as improving clarity, and inappropriate uses like generating core arguments or "composite voice" prose.  
* **Week 7: Code and Data Analysis Assistance.** We focus on using AI for code generation and debugging in R or Python, with a heavy emphasis on verification strategies to catch subtle logic errors.  
* **Week 8: Emerging Applications—Qualitative Analysis and Study Design.** This week addresses experimental uses, including AI’s role in qualitative coding and the epistemological tensions it creates within interpretive traditions.  
* **Week 9: Building Sustainable AI Practices.** Learners develop personal policies to avoid skill atrophy and over-reliance, incorporating bias awareness and environmental considerations into their long-term workflows.  
* **Week 10: Integration, Teaching, and Looking Forward.** The final week synthesizes the research lifecycle, positioning participants to mentor others and contribute to evolving disciplinary norms regarding AI.

## **Gemini**

* **Week 1: Unlocking the Black Box – Probability, Not Truth.** We demystify LLMs as "probabilistic token predictors" rather than truth engines, explaining how next-token prediction inherently prioritizes plausibility over factual accuracy.  
* **Week 2: The Art of Inquiry – Prompt Engineering as Research Methodology.** This week reframes prompts as rigorous sets of constraints—using techniques like Few-Shot and Chain of Thought (CoT) to align the model’s latent space with research intent.  
* **Week 3: Cognitive Ethics – Centaurs, Cyborgs, and Offloading.** Learners develop a "Cognitive Risk Policy" to distinguish between "Safe Offloading" (formatting/debugging) and "Unsafe Offloading" (interpretive analysis) that risks skill atrophy.  
* **Week 4: The Literature Review – Synthesis Over Search.** We emphasize that LLMs are not search engines, teaching workflows that combine human-led retrieval with AI-assisted synthesis to avoid "Frankenstein" citations.  
* **Week 5: Ideation and Hypothesis – The "Hypogenic" Researcher.** The AI acts as a "Socratic Sparring Partner," using adversarial prompting to identify cross-disciplinary connections and test the robustness of human-generated theories.  
* **Week 6: Methodological Support – Coding, Quant, and Qual.** This session explores the "No-Code" revolution for data cleaning while warning against using AI for primary inductive coding in qualitative research.  
* **Week 7: Dissemination – Writing, Voice, and Audience.** Participants master "Style Transfer" to adapt technical findings for policy-makers or journalists while stripping away the generic, buzzword-laden "AI voice."  
* **Week 8: The Peer Review Simulation – Ethics and Utility.** We discuss the ethical boundaries of AI in evaluation, teaching its use as a "Pre-Submission Stress Test" to anticipate critiques without offloading the reviewer's duty.  
* **Week 9: Epistemic Security – Model Collapse and the Future of Truth.** This week examines systemic risks like "Model Collapse"—where models trained on synthetic data degrade—and frames human verification as the new premium in research.  
* **Week 10: Governance – Designing Your Personal AI Manifesto.** The course culminates in the creation of a personal "Lab Manifesto," codifying individual "Red Lines" and transparency standards for long-term scholarly integrity.

# **Format**

**10 weeks, two emails per week**

* **Email 1 (Monday, Spark)**: 10–15 minutes, one concrete exercise.  
* **Email 2 (Thursday, Anchor)**: 5–10 minutes, debrief \+ durable habit \+ one “prompt worth keeping.”

**Midpoint check-in email**: after Week 5\.

\---

Sign up at any time, fully asynchronous \- opportunity to share feedback by email, and questions/lessons learned on GitHub Discussion threads

# **Weekly outline**

## **Week 1 — Orientation & Baselines: Probability, Not Truth (in real context)**

### **Email 1A (Spark)**

**Subject:** 🧠1A. Baseline: what do you trust AI for (and why)?

**Purpose**

* Establish psychological safety and a personal baseline.  
* Begin capability-aware planning (what to use AI for, and why).

**Core concepts**

* LLMs have hugely accelerated some areas of work  
* LLMs generate plausible continuations, not truth.  
* Confidence is a style feature.  
* Different models behave differently; treat them as distinct collaborators.

**Exercise (10–15 min): AI autobiography \+ tool comparison**

1. **AI autobiography (6 bullet points):**  
     
   * current uses  
   * perceived benefits  
   * pitfalls experienced  
   * biggest worry  
   * current red lines / tasks you refuse to outsource  
   * goals for this course

   

2. **Tool comparison:** ask 2–3 tools the *same* question on a topic you know well. Suggested prompts:  
     
   * “Explain X in plain language for a smart non-expert.”  
   * “Recommend 6 foundational readings for X and explain why each matters.”  
   * “Propose 3 plausible hypotheses about X and how you’d test them.”

   

   **Note**: what was helpful? what was wrong? what was persuasive-but-flimsy?

   

   

**What AI should I use?**

In this course, we generally do not recommend specific models \- because this becomes outdated very fast, but also because the choice of model will depend on your preferences, budget, language etc. It is worth checking some of the main providers (e.g. OpenAI’s ChatGPT, Google’s Gemini, Anthropic’s Claude) as well as some of the leading Open Source models (e.g. Kimi, Minimax, Deepseek, GLM, Mistral). You can find many leaderboards of models that can help guide your exploration, e.g., [https://artificialanalysis.ai/leaderboards/models](https://artificialanalysis.ai/leaderboards/models) 

As you get started, you might want to check out a provider that gives you access to many models at once, e.g. [https://t3.chat/](https://t3.chat/). Most of the activities in this course will work without having to pay for any subscription, if you are willing to switch between providers.

**Add to Prompt Library (Clarify & Specify): ‘Clarification Suffix’**

In the next email, we will explore *how* LLMs actually come up with these responses.

---

### **Email 1B (Anchor)**

**Subject:** 🧠1B. What you probably noticed: confidence, drift, and context

**Purpose**

* Install a correct mental model without toy simplifications.

**Core concepts**

* LLMs predict how a text would continue \- word-by-word.  
  * Tokenisation, then learning patterns of associations  
* “Stochastic Parrot” vs “emergent reasoning” debate (introduced neutrally).  
* Next-token prediction is **context-conditioned** (long text, not just a sentence).  
* Training data and knowledge cut-offs shape (i.e. bias) outputs.

**Exercise (5–8 min): Context continuation game**

1. Take a paragraph you wrote (intro, methods, email). Delete the next 1–2 sentences.  
2. Ask the model to continue **without adding new factual claims**.  
3. Compare: where did it match style but flatten nuance or sneak in new claims?

**Add to Prompt Library (Writing & Voice): ‘Voice Matcher (No New Claims)’**

Task: Continue the following text as if you were the same author.

Constraints:

1. Match tone, vocabulary, sentence length, and level of formality.  
2. **Do not introduce any new factual claims, citations, or external knowledge** that are not already present in the provided text.  
3. If you feel a new claim would be useful, insert a placeholder like: **\[NEEDS SOURCE / NEW CLAIM\]** instead of stating it.  
4. If you are uncertain about whether something counts as a new claim, mark it with **\[UNCERTAIN\]**.

Output: Provide only the continuation.

**Further exploration**

* Notice “sounds right” vs “constrained by evidence/context.”

---

## **Week 2 — Confident Errors: Hallucination, Sycophancy, Epistemic Vigilance**

### **Email 2A (Spark)**

**Subject:** \[GAIR\] The citation your AI just invented

**Purpose**

* Turn citation hallucinations into a detection reflex.

**Core concepts**

* Models can produce citation-shaped text without retrieval.  
* Unique combinations (full references) are failure-prone.

**Exercise (10–15 min): Frankenstein Hunt**

1. Ask for 6 citations supporting a niche claim you know.  
2. Verify existence and whether each supports the claim.  
3. Label: real / fabricated / Frankenstein / misattributed / outdated.

**Add to Prompt Library (Checks & Uncertainty): ‘Citation Discipline (No Fake Quotes)’**

Provide **up to 6** citations relevant to my claim.

For each citation, include:

1. The **exact claim** it is meant to support (1 sentence).  
2. A **verification plan**: what I should search for (author/year/title keywords) and where (publisher site, Google Scholar, library search).  
3. A **risk flag**: “HIGH RISK OF HALLUCINATION” if you are not retrieving sources.

Critical constraint:

* **Do NOT invent quotes**. If you do not have the paper text in front of you (because I did not provide it), you must not provide verbatim passages.  
* If you are uncertain whether a citation exists, say so explicitly.

---

### **Email 2B (Anchor)**

**Subject:** \[GAIR\] Why it tells you what you want to hear (and when it’s worth using)

**Purpose**

* Explain sycophancy \+ teach the key decision rule: generation–verification asymmetry.

**Core concepts**

* RLHF can push toward pleasing, agreeable responses.  
* Sycophancy is managed by adversarial prompts and explicit constraints.  
* **Asymmetry Rule:** AI is best where generation is costly and verification is cheap.  
* Search grounding helps retrieval but not judgment.

**Exercise (5–8 min): High-ROI audit**

1. List 5 tasks you do often.  
2. Rate each: cost of generation for you; cost of verification for you; harm if wrong.  
3. Identify: 2 high-ROI uses \+ 1 danger-zone task.

**Add to Prompt Library (Checks & Uncertainty): ‘Uncertainty Check \+ Verification Methods’**

Answer my question, but you must also do the following:

1. List the **three parts of your answer you are least confident about**.  
2. For each, propose a **specific verification method** I can use (e.g., “search Google Scholar for X; check the methods section for Y; look up the official policy on Z”).  
3. For each, tell me what outcome would falsify your claim.

Constraints:

* If you are not using retrieval tools and I did not provide sources, do not present citations as confirmed facts.

**Sycophancy mini-demo (2 minutes)**

* Prompt 1: “Praise this idea; assume it’s correct.”  
* Prompt 2: “Attack this idea; assume it’s flawed.”  
* Compare tone and specificity.

**Further reading:**

* https://openai.com/index/why-language-models-hallucinate/

---

## **Week 3 — Prompting as Methodology \+ Thinking Modes (without mysticism)**

### **Email 3A (Spark)**

**Subject:** \[GAIR\] Prompt hacks are mostly theatre

**Purpose**

* Prompting as specification and interaction, not magic.

**Core concepts**

* Most “hacks” matter less; clarity matters more.  
* Roles/personas and few-shot examples calibrate intent.  
* Thinking modes can help on hard tasks; they don’t guarantee truth.

**Exercise (10–12 min): Iteration ladder** Pick a real task and run 4 prompts:

1. Vague  
2. Constrained  
3. Role-based  
4. Few-shot example

**Add to Prompt Library (Clarify & Specify): ‘Standard Protocol Template’**

Role: \[e.g., Expert methodologist / skeptical reviewer / writing coach\]

Task: \[Action verb \+ object\]

Context:

* My field: \[ \]  
* Audience: \[ \]  
* Goal: \[ \]  
* Constraints (time/length): \[ \]

Output format: \[e.g., bullets; table; numbered steps\]

Success criteria:

* \[e.g., must include assumptions; must include alternatives; must include risks\]

Negative constraints (do not):

* Do not invent citations.  
* Do not add new factual claims unless flagged.  
* Do not flatter; be direct.

Before answering:

1. Ask me up to 3 clarifying questions.  
2. Then provide the output.

---

### **Email 3B (Anchor)**

**Subject:** \[GAIR\] A small prompt repertoire beats 100 clever prompts

**Purpose**

* Provide a durable prompt starter pack.  
* Introduce “checkable intermediate outputs” as the safe alternative to demanding chain-of-thought.

**Core concepts**

* Few-shot calibrates output style.  
* Ensembles increase perspective diversity but don’t prove truth.  
* For “thinking,” request intermediate artifacts you can verify: assumptions, test cases, decision trees.

**Deliverable: Prompt Starter Pack (participants copy the ones they’ll actually use)**

**1\) Clarifier**

Before answering, ask 3 clarifying questions. Then give me two alternative approaches and explain the trade-offs.

**2\) Transformer (no new claims)**

Transform the following content into \[format\]. Constraints: keep meaning identical; do not add claims; flag anything that would require external knowledge.

**3\) Critic (logic-only)**

Critique only the reasoning/structure; do not rewrite; list missing steps and ask clarifying questions.

**4\) Red team / failure modes**

Identify plausible failure modes and how to detect them quickly.

**5\) Planner (with checkpoints)**

Produce a plan with checkpoints; for each checkpoint include acceptance criteria and failure signals.

**Add to Prompt Library (Checks & Uncertainty): ‘Intermediate Output Request’**

Do NOT give me a final answer yet.

First produce:

1. A list of **assumptions** you are making.  
2. A list of **intermediate outputs** you would need to be confident (e.g., a table, a decision tree, a checklist).  
3. A minimal **test plan**: 3 checks I could run to validate the final answer.

Only after that, provide the final answer.

---

## **Week 4 — Literature & Synthesis: Triangulation \+ Grounding (RAG) \+ Attribution**

### **Email 4A (Spark)**

**Subject:** \[GAIR\] Chatbots are not search engines

**Purpose**

* Use AI in literature work without outsourcing reading or flattening debates.

**Core concepts**

* Chat ≠ search. Grounding improves retrieval, not judgment.  
* Homogenisation risk: bland consensus summaries.

**Exercise (10–15 min): Triangulation test (use a paper you must read anyway)**

1. Choose one paper you need for current work.  
2. Ask AI for: 5 claims; 3 uncertainties; 5 methods details to inspect.  
3. Compare with: abstract \+ skim figures/tables \+ your own judgment.  
4. Note: what did AI miss? what did it overstate?

**Add to Prompt Library (Literature & Synthesis): ‘Paper Extraction Protocol’**

I am working with the following paper (I may paste the abstract or excerpts).

Task: Extract information **without summarizing**.

Output exactly:

1. **Five central claims** (1 sentence each).  
2. **Three limitations/uncertainties** explicitly stated by the authors.  
3. **Five specific methods details** I should inspect to judge validity (e.g., sampling, measures, exclusion criteria, model specification).

Constraints:

* If I did not provide the paper text, do not pretend you read it.  
* If you are unsure, mark items with \[UNCERTAIN\].

---

### **Email 4B (Anchor)**

**Subject:** \[GAIR\] Grounding helps retrieval—not judgment

**Purpose**

* Explain RAG/search grounding and how to use it defensibly.

**Core concepts**

* RAG/search tools are better at traceability.  
* Still weak at weighting evidence and identifying subtle caveats.  
* For systematic reviews, stricter workflows are needed.

**Exercise (5–8 min): Evidence linking without hallucinated quotes**

1. Pick 3 claims you might rely on.  
2. Find supporting text in a source you actually have open.  
3. Save one receipt if the claim matters.

**Add to Prompt Library (Checks & Uncertainty): ‘Evidence Linker (Source-Only)’**

I will provide source text (abstract, excerpt, notes, or pasted passage).

Task: For each claim you produce, you must:

1. Quote a **short exact excerpt** from the text I provided (max 1–2 sentences).  
2. Explain why that excerpt supports the claim.

If I do NOT provide source text:

* Do NOT fabricate quotes.  
* Instead, give me a lookup plan: where to search, what keywords to use, and what passage would count as support.

**Optional: disagreement extractor prompt**

From the text provided, list:

* areas of disagreement/controversy in the literature (if mentioned)  
* competing explanations  
* what evidence each side typically relies on

---

## **Week 5 — Ideation & Creativity: Better ideas, more convergence**

### **Email 5A (Spark)**

**Subject:** \[GAIR\] Use AI for resistance, not autopilot

**Purpose**

* Use AI as sparring partner; resist homogenisation.

**Core concepts**

* AI can raise individual quality but increase convergence.  
* Useful for critique and stress testing.

**Exercise (10–15 min): Reviewer \#2 stress test**

1. Paste your question/abstract.  
2. Ask for fatal flaws \+ fixable weaknesses.  
3. Write a human rebuttal for top 3\.

**Add to Prompt Library (Checks & Uncertainty): ‘Harsh Reviewer (Field-Specific)’**

Adopt the persona of a skeptical, senior reviewer in **my field**.

Input: \[paste text\]

Output:

1. Three **fatal flaws** (logic/design/inference) that would justify rejection.  
2. Three **fixable weaknesses** (presentation/clarity/controls).  
3. The **single most decisive piece of evidence** that would change your mind.

Constraints:

* Be direct. No flattery.  
* If you need field context, ask up to 3 clarifying questions first.

---

### **Email 5B (Anchor)**

**Subject:** \[GAIR\] Mean reversion of ideas: protect originality

**Purpose**

* Install a divergence routine.

**Core concepts**

* Convergence is structural.  
* Divergence is a habit.

**Exercise (5–8 min): De-convergence protocol (pick one)**

* boundary cases  
* rival hypotheses  
* reverse argumentation

**Add to Prompt Library (Checks & Uncertainty): ‘Divergence Generator (Variance Injection)’**

Do not agree with me. Instead, your job is to increase **idea variance**.

Input: \[my hypothesis/argument\]

Output:

1. Three **rival hypotheses** that could explain the same pattern.  
2. Three **boundary cases** where my hypothesis would fail.  
3. Three **theoretical lenses** (mutually incompatible if possible) that would interpret the same evidence differently.  
4. The **crucial test** that would distinguish my hypothesis from the rivals.

Constraint: be specific and concrete; no generic “more research needed.”

---

## **Midpoint check-in (after Week 5B)**

**Subject:** \[GAIR\] Halfway: what’s changed in your practice?

**Purpose**

* Re-anchor, reduce dropout, invite feedback.

**Core message**

* No need to catch up; each email stands alone.  
* Next half focuses on methods integrity, writing boundaries, governance, workflows, SOP.

**Reflection prompt (reply-to-email):**

* “One habit you’ve started—or one temptation you’ve noticed—since Week 1?”

---

## **Week 6 — Methods & Analysis: Jagged frontier, broken legs, p-hacking-by-accident**

### **Email 6A (Spark)**

**Subject:** \[GAIR\] P-hacking by accident: when iteration becomes a confound

**Purpose**

* Reframe risk correctly: not only wrong code, but **cheap analytic flexibility** \+ post-hoc narratives.

**Core concepts**

* Jagged frontier: uneven capability.  
* AI lowers cost of trying alternatives → forking paths.  
* Data familiarity prevents “broken legs.”

**Exercise (10–15 min): Quant OR Qual track**

**Quant track: Forking-path map \+ minimal pre-commitment**

1. Ask AI to list reasonable analytic choices and decision points.  
2. Pick one primary plan and write a one-sentence pre-commitment.  
3. Run a “broken legs” sanity scan (3–5 checks).

**Qual track: Intimacy \+ codebook discipline**

1. Manually code a short excerpt.  
2. Ask AI to code the same excerpt using your codebook.  
3. Compare: flattening, missed nuance, overconfidence.

**Add to Prompt Library (Methods & Analysis): ‘Forking Path Mapper’**

I am analyzing data for the question: \[question\]

Context:

* Design: \[experimental/observational\]  
* Outcome(s): \[ \]  
* Key predictors/conditions: \[ \]  
* Planned model family: \[e.g., linear regression / mixed model / logistic / ANOVA / thematic coding\]

Task: Produce a **Forking Path Map** with decision points.

Output format:

* A numbered list of **decision points** (e.g., exclusion criteria, transformations, covariates, model specification, coding granularity).  
    
* For each decision point:  
    
  1. 2–4 reasonable options  
  2. what assumption each option makes  
  3. how each option could change conclusions (directionally)  
  4. which option is most defensible **a priori** and why

Constraints:

* Do not invent data facts you don’t know.  
* Ask clarifying questions if missing key info.

**Add to Prompt Library (Methods & Analysis): ‘Minimal Pre-commitment Wording’**

Given my question and design, help me write **one sentence** that clearly states my primary analysis choice and what would justify switching.

The sentence must have this structure:

* “Primary analysis will be \[X\] unless \[predefined condition Y occurs\], in which case we will \[Z\].”

Ask up to 3 clarifying questions if needed.

**Add to Prompt Library (Methods & Analysis): ‘Broken Legs Checklist (Data Familiarity)’**

Before doing any substantive analysis, generate a **minimal data familiarity checklist** for this dataset.

Output:

1. 10 “broken legs” checks that are cheap and catch obvious issues (e.g., impossible values, coding inversions, duplicates, missingness patterns, unit mismatches).  
2. For each check: what failure looks like, and what I should do if I see it.  
3. Keep it brief and practical; no generic advice.

---

### **Email 6B (Anchor)**

**Subject:** \[GAIR\] If you don’t look at the data, you can’t spot broken legs

**Purpose**

* Make integrity practical. Introduce multimodal as an ROI win.

**Core concepts**

* Cheap checks over rituals.  
* Multimodal extraction is high-ROI where verification is cheap.  
* Synthetic/simulated data: useful for testing pipelines, dangerous for inference.

**Exercise (8–10 min): Multimodal digitisation**

1. Screenshot a table/chart from a PDF you can’t copy-paste (non-sensitive).  
2. Ask model to transcribe to CSV and mark uncertain cells.  
3. Spot-check 5 random cells.

**Add to Prompt Library (Methods & Analysis): ‘Multimodal Transcriber (No Guessing)’**

Task: Convert the attached image into a clean CSV.

Constraints:

1. **Do not guess**. If a value is unclear, write **\[UNCLEAR\]**.  
     
2. Preserve the exact row/column structure.  
     
3. After the CSV, list:  
     
   * the 5 cells you are least confident about  
   * what would let you resolve them (zoom, higher-res, legend clarification)

**Add to Prompt Library (Methods & Analysis): ‘Silent Failure Modes’**

I am about to trust this analysis output: \[paste output or describe analysis\].

Task: Identify **silent failure modes**—ways this could be wrong without obvious errors.

Output:

1. 8–10 plausible silent failure modes  
2. For each: a cheap check I can run (ideally under 5 minutes)  
3. Which failures are most likely vs most harmful

---

## **Week 7 — Writing, voice, disclosure, peer review boundaries**

### **Email 7A (Spark)**

**Subject:** \[GAIR\] Writing is thinking: keep cognitive ownership

**Purpose**

* Use AI for clarity without outsourcing synthesis/stance.

**Exercise (10–12 min): Two-pass writing**

* Pass 1: logic-only critique.  
* You revise.  
* Pass 2: style smoothing with “no new claims \+ highlight changes.”

**Add to Prompt Library (Writing & Voice): ‘Logic-only Critique (No Rewrite)’**

Read the following draft.

Constraints:

* Do NOT rewrite any sentences.  
* Do NOT comment on grammar or style.

Task:

1. Identify 3 places where the logical connection is missing or weak.  
2. For each, ask me one clarifying question.  
3. Identify one potential overclaim and suggest how to qualify it *without weakening the argument unnecessarily*.

**Add to Prompt Library (Writing & Voice): ‘Clarity Rewrite With Claim Guardrails’**

Rewrite the text to improve clarity and flow **without changing the meaning**.

Constraints:

1. Do not add new factual claims.  
     
2. Do not add citations.  
     
3. After rewriting, produce a “Claim Change Report”:  
     
   * List any sentence where you might have introduced a new claim.  
   * If none, state: “No new claims introduced.”

---

### **Email 7B (Anchor)**

**Subject:** \[GAIR\] Peer review boundaries \+ disclosure without drama

**Purpose**

* Clarify what is acceptable in self-review vs confidential peer review.

**Add to Prompt Library (Checks & Uncertainty): ‘Policy Checker’**

I am considering using AI for: \[task\].

Ask me:

1. What data/material would be shared?  
2. Whether it is confidential or unpublished?  
3. Which publisher/funder/institution policies apply?

Then propose a safe alternative workflow if the answer suggests confidentiality risk.

**Add to Prompt Library (Writing & Voice): ‘Stance Keeper (Avoid Flattening)’**

Analyze my draft for “voice flattening.”

Output:

1. Identify 5 places where the text becomes generic or overly hedged.  
2. For each, propose a revision that preserves my stance **without adding claims**.  
3. Flag any sentence that sounds like AI boilerplate.

---

## **Week 8 — Governance: privacy, policy, local/cloud, resource proportionality**

### **Email 8A (Spark)**

**Subject:** \[GAIR\] The policies that already govern you

**Exercise (10–15 min): Policy hunt**

* Locate applicable policies (institution, funder, target journals, professional body).  
* Note ambiguities.

**Add to Prompt Library (Clarify & Specify): ‘Data-Class Prompt Rewriter’**

I want to use AI for \[task\].

First ask me to classify the input as:

* Public  
* Internal  
* Sensitive (e.g., participant data, unpublished results)  
* Confidential (e.g., peer review, identifiable transcripts)

Then rewrite my prompt to:

* remove identifiers  
* replace rare combinations with placeholders  
* preserve the analytic intent

Finally, list residual risks.

---

### **Email 8B (Anchor)**

**Subject:** \[GAIR\] Don’t bring a tank to a wrestling match

**Core concepts**

* Local vs cloud trade-offs.  
* “Free” often means value extraction.  
* Resource proportionality: smaller models for small tasks.

**Add to Prompt Library (Checks & Uncertainty): ‘Risk Scanner (De-identification)’**

I have a dataset with the following column headers and examples: \[paste headers \+ 1–2 example rows with fake data\]

Task:

1. Identify which columns or combinations could identify a person (including rare combinations).  
2. Propose a de-identification strategy for each (drop, bin, generalize, hash, redact free text).  
3. List residual re-identification risks.  
4. Suggest what can be safely shared as a derived summary instead.

---

## **Week 9 — Integration: workflows, agents/APIs, supervision**

### **Email 9A (Spark)**

**Subject:** \[GAIR\] From ad hoc to designed: map your workflow (and try one bounded agent)

**Purpose**

* Convert principles into workflow.  
* Deliver objective (3) via a concrete, bounded agent/API-style task.

**Exercise (10–15 min): Workflow map \+ one agentic micro-project**

1. Workflow map: list 10 tasks; classify human-only / AI-supported / AI-outsourced.  
2. For each AI-supported step: write one cheap check.  
3. Choose ONE bounded agentic micro-project below.

**Agentic micro-project (tool-agnostic option A: “bounded literature extractor”)**

* Inputs: 3–5 PDFs you already have.  
* Output: a table with columns: claim; evidence location; methods note; limitation; your confidence.  
* Acceptance criteria: every claim must have a page/section pointer or be marked “needs verification.”

**Agentic micro-project (tool-agnostic option B: “bounded admin agent”)**

* Inputs: a committee agenda or project plan.  
* Output: action list with owners, deadlines, risks.  
* Acceptance criteria: no invented facts; asks clarifying questions.

**Add to Prompt Library (Integration): ‘Human-in-the-Loop Spec’**

I want to use AI/agents for the task: \[task\].

Produce a Human-in-the-Loop specification with:

1. Inputs (what I will provide)  
2. Outputs (what format)  
3. Checkpoints (where a human must review)  
4. Acceptance criteria (what counts as “done”)  
5. Failure modes (how this could go wrong)  
6. Cheap checks at each checkpoint

Ask up to 3 clarifying questions first.

**Add to Prompt Library (Integration): ‘Agent Prompt (Bounded, With Acceptance Criteria)’**

You are acting as a bounded research assistant.

Goal: Create a structured extraction table from the documents I provide.

Constraints:

* Do not invent citations or quotes.  
* If you cannot locate support in the provided documents, mark the entry **NEEDS VERIFICATION**.  
* Ask clarifying questions if my task definition is ambiguous.

Output format: Provide a table with columns:

* Claim (1 sentence)  
* Evidence pointer (page/section from provided docs)  
* Method detail to inspect  
* Limitation/caveat  
* Confidence (Low/Med/High) *with a short reason tied to evidence presence*

---

### **Email 9B (Anchor)**

**Subject:** \[GAIR\] The training paradox: what your students can’t skip

**Exercise (5–8 min): Supervision rules**

* Draft 6 rules: manual prerequisites, allowed AI supports, required disclosures, fork-control norm.

**Add to Prompt Library (Teaching/Admin): ‘Trainee Policy Generator (Practical)’**

Draft a short AI use policy for a PhD student working on \[topic\].

Include:

1. Three tasks they must master manually before using AI (and why).  
2. Three tasks where AI support is allowed (with constraints).  
3. A fork-control rule that prevents accidental p-hacking-by-accident.  
4. A data confidentiality rule.  
5. What they must disclose in write-ups.

Keep it to \~12 bullet points, operational and concrete.

---

## **Week 10 — Consolidation: SOP \+ staying current**

### **Email 10A (Spark)**

**Subject:** \[GAIR\] Your AI SOP: boring, reusable, real

**Purpose**

* Convert the course into a document you can use and share.

**Exercise (15–20 min): Draft your SOP** The SOP must include:

1. Green uses (default allowed)  
2. Amber uses (allowed with checks)  
3. Red lines (never)  
4. Data handling rules  
5. Peer review boundary rules  
6. Analysis integrity rules (fork-control \+ data familiarity)  
7. Your 8–12 best prompts  
8. Disclosure defaults

**Add to Prompt Library (Capstone): ‘SOP Builder (Operational, With Examples)’**

I want you to help me draft a one-page AI Standard Operating Procedure (SOP) for research use.

First, ask me up to **8** short questions to capture:

* my field and common tasks  
* data sensitivity  
* writing expectations  
* typical analyses  
* supervision responsibilities  
* what I consider unacceptable

Then produce the SOP with this structure:

**1\) Purpose (2–3 sentences)** **2\) Green zone: Allowed by default**

* bullet list of allowed uses with 1 example each

**3\) Amber zone: Allowed only with checks**

* for each amber use:  
    
  * what check I must do (cheap check)  
  * what I must not do  
  * what “save a receipt” looks like

**4\) Red zone: Prohibited**

* clear bullets with short rationales

**5\) Data handling rules**

* public/internal/sensitive/confidential defaults

**6\) Analysis integrity**

* fork-control norm (pre-commitment language)  
* broken legs checklist

**7\) Peer review boundary**

**8\) Disclosure defaults**

* a short default statement template

Constraints:

* Keep it operational (no philosophy).  
* No generic filler.  
* Where uncertain, ask.

---

### **Email 10B (Anchor)**

**Subject:** \[GAIR\] Staying current without chasing tools

**Purpose**

* Build a durable habit for updating beliefs.

**Exercise (5–8 min): Quarterly calibration ritual**

1. Choose 2 benchmark tasks relevant to you (one low-stakes, one high-stakes).  
2. Define what counts as “pass.”  
3. Schedule a quarterly re-test.

**Add to Prompt Library (Checks & Uncertainty): ‘Benchmark Designer (Task-Specific)’**

**Optional further exploration (macro risks, brief pointers)**

* Deskilling/skill atrophy  
* Model collapse  
* Literature slop/fraud  
* Centralisation/commercialisation vs openness  
* Existential risk narratives (kept optional)

**Final interaction prompt (reply-to-email):**

* “What’s one SOP rule you’d hand to a PhD student?”

### **Scaffolded record-keeping: Personal Prompt Library**

Participants receive a link at enrolment to a **read-only Google Doc template**.

* **Action:** If you don’t maintain a prompt library yet, “click here to copy the template into your workspace.”  
* **Goal:** Curation, not collection. By Week 10: \~10 prompts you actually reuse.

**Suggested sections:**

1. Clarify & Specify  
2. Checks & Uncertainty  
3. Literature & Synthesis  
4. Methods & Analysis  
5. Writing & Voice  
6. Teaching/Admin (optional)

# **Prompt Library**

1. Clarify & Specify

***Clarification suffix***

You are my research assistant. Before answering, ask me **exactly three** clarifying questions to understand my context, constraints, and intended output.

Then, list **two** plausible interpretations of my request (A and B) in one sentence each.

Only after I answer, produce the final output.

Important: if you lack key information, do not guess—ask.

NB: Many AI chat interfaces allow you to specify custom instructions. You might want to put a version of this in there.

2. Checks & Uncertainty

***Benchmark designer:*** 

I want to evaluate whether a new model/tool is ready for this task: \[task\].

Design a benchmark with:

1. **Easy sanity check** (should always pass)  
2. **Hard case** (requires real reasoning or careful constraint-following)  
3. **Trap case** (designed to trigger hallucination/sycophancy or false confidence)

For each case, specify:

* the exact prompt  
* what a “pass” looks like  
* common failure signatures  
* a cheap verification step

Finally, suggest how I should record results in 3 bullet points.

3. Literature & Synthesis  
4. Methods & Analysis  
5. Writing & Voice  
6. Teaching/Admin (optional)