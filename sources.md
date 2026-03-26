# References & further reading

Weekly references, sources, and further reading for the course. Each email links to its week's section.

---

## Week 1 — What LLMs are (and aren't)

**References**

- Summerfield, C. (2025). *These Strange New Minds: How AI Learned to Talk and What It Means*. Viking. — A neuroscientist and AI researcher's accessible account of how LLMs work and what their rise means; recommended in the Thursday email as an entry point to the "understanding or pattern-matching?" debate.

**Further reading**

- 3Blue1Brown. (2024). Large language models explained briefly [Video]. YouTube. https://www.youtube.com/watch?v=LPZh9BOjkQs — Short visual explainer of next-token prediction, training, RLHF, and attention. Best starting point if you want to see how LLMs work under the hood.
- 3Blue1Brown. (2024). Transformers, the tech behind LLMs [Video]. YouTube. https://www.youtube.com/watch?v=wjZofJX0v4M — Deeper visual walkthrough of transformer architecture ... if you really want to go beyond the basics.
- Wolfram, S. (2023, February 14). What is ChatGPT doing... and why does it work? https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/ — Long (~25,000 words) but thorough essay bridging technical and general audiences. Starts accessibly, gets progressively more technical. For the genuinely curious.
- OpenAI. (2025, April 30). Sycophancy in GPT-4o: What happened and what we're doing about it. https://openai.com/index/sycophancy-in-gpt-4o/ — OpenAI's post-mortem on a model update that over-optimised for user approval, producing a model that was "overly supportive but disingenuous." Background to the sycophancy discussion in this email.
- Georgetown Law Institute for Technology Law & Policy. (2025, July 30). Tech brief: AI sycophancy & OpenAI. https://www.law.georgetown.edu/tech-institute/insights/tech-brief-ai-sycophancy-openai-2/ — Policy analysis of how reduced safety staffing, compressed testing, and marketplace incentives led to the GPT-4o sycophancy incident, including documented harms such as users being encouraged to stop medication.
- Raghavan, P. (2024, February 23). What happened with Gemini image generation. *Google Blog*. https://blog.google/products/gemini/gemini-image-generation-issue/ — Google's explanation of how diversity tuning in Gemini's image generation overcompensated, producing historically inaccurate images. Background to the example mentioned in this email.

---

## Week 2 — Confident errors: hallucination and sycophancy

**References**

- OpenAI. (2025). Why language models hallucinate. https://openai.com/index/why-language-models-hallucinate/ — OpenAI's own explanation of the problem, arguing that standard training rewards guessing over expressing uncertainty.
- Bergstrom, C. T., & West, J. D. (2025). *Modern-day oracles or bullshit machines?* [Free online course]. https://thebullshitmachines.com/ — From the creators of *Calling Bullshit*: 18 short lessons on critical thinking about AI, framing LLMs as "both powerful tools, and mindless bullshit machines." Embodies the "epistemic vigilance" spirit mentioned in the Thursday email, in highly accessible form.

**Further reading**

- Rozear, H. (2026, January 5). It's 2026. Why are LLMs still hallucinating? Duke University Libraries Blog. https://blogs.library.duke.edu/blog/2026/01/05/its-2026-why-are-llms-still-hallucinating/ — Accessible overview of four core reasons LLMs hallucinate, written from a university library perspective.
- Hutson, M. (2026, March 11). AI sycophancy: Why chatbots agree with you. *IEEE Spectrum*. https://spectrum.ieee.org/ai-sycophancy — On why language models abandon correct answers to please users, and research into teaching AI to push back.

---

## Week 3 — Prompting, ideation, and the convergence trap

**References**

- Meincke, L., Nave, G., & Terwiesch, C. (2025). ChatGPT decreases idea diversity in brainstorming. *Nature Human Behaviour*, *9*(6), 1107–1109. https://doi.org/10.1038/s41562-025-02173-x — Using ChatGPT enhanced average idea creativity but reduced diversity across participants' ideas. 
- Hao, Q., Xu, F., Li, Y., & Evans, J. A. (2026). Artificial intelligence tools expand scientists' impact but contract science's focus. *Nature*, *649*, 1237–1243. https://doi.org/10.1038/s41586-025-09922-y — Analysis of 41 million papers: AI-augmented researchers publish more and are cited more, but AI adoption narrows research diversity and reduces collaboration.

**Further reading**

- Harvey, G. (2026, March 19). The AI skill that replaced prompt engineering (and you're already using it). *The Neuron*. https://www.theneuron.ai/explainer-articles/the-ai-skill-that-replaced-prompt-engineering-and-youre-already-using-it/ — Argues that metacognition (clear thinking about what you want) has replaced prompt engineering: "The models got good enough that you don't need to trick them anymore."
- Jiang, L., Chai, Y., Li, M., Liu, M., Fok, R., Dziri, N., ... & Choi, Y. (2025). Artificial hivemind: The open-ended homogeneity of language models (and beyond). *arXiv preprint.* https://doi.org/10.48550/arXiv.2510.22954 - provides evidence that simple prompts result in very similar outputs within and across models, e.g. prefering "time is a river" as *the* metaphor about time.

---

## Week 4 — Grounded tools: working with your own sources

**References**

- Pope, C. (2025, December 1). Using NotebookLM for academic research. https://catherinepope.com/posts/using-notebooklm-for-academic-research/ — Practical guide to using NotebookLM for searching your own documents, finding forgotten quotes, and identifying literature gaps.
- van de Schoot, R., de Bruin, J., Schram, R., Zahedi, P., de Boer, J., Weijdema, F., Kramer, B., Huijts, M., Hoogerwerf, M., Ferdinands, G., Harkema, A., Willemsen, J., Ma, Y., Fang, Q., Hindriks, S., Tummers, L., & Oberski, D. L. (2021). An open source machine learning framework for efficient and transparent systematic reviews. *Nature Machine Intelligence*, *3*(2), 125–133. https://doi.org/10.1038/s42256-020-00287-7 — Introduces ASReview, the open-source active-learning tool for systematic review screening mentioned in the Thursday email. Note that this is *not* LLM-based.

**Further reading**

- Merritt, R. (2025, January 31; updated October 9, 2025). What is retrieval-augmented generation, aka RAG? *NVIDIA Blog*. https://blogs.nvidia.com/blog/what-is-retrieval-augmented-generation/ — Clear explainer with many good examples (though you will likely want to ignore the details on how to roll this out in an organisation)

---

## Week 5 — Writing with AI

**References**

- Bangert-Drowns, R. L., Hurley, M. M., & Wilkinson, B. (2004). The effects of school-based writing-to-learn interventions on academic achievement: A meta-analysis. *Review of Educational Research*, *74*(1), 29–58. https://doi.org/10.3102/00346543074001029 — Meta-analysis of 48 studies finding that writing-to-learn activities produce a reliable positive effect on achievement, with metacognitive prompts amplifying the benefit.
- Prakash, A., Aggarwal, S., Varghese, J. J., & Varghese, J. J. (2025). Writing without borders: AI and cross-cultural convergence in academic writing quality. *Humanities and Social Sciences Communications*, *12*(1), Article 1058. https://doi.org/10.1057/s41599-025-05484-6 — Argues that AI-assisted convergence in academic writing style may be a net positive internationally, levelling the playing field for non-native English speakers.
- Ghods, K., & Liu, P. (n.d.). *Evidence against LLM homogenization in creative writing*. https://kiaghods.com/assets/pdfs/LLMHomogenization.pdf — Unpublished class project arguing that LLM stylistic homogenisation largely disappears when models are given context. Weak evidence so far, but maybe a template for testing the convergence narrative more rigorously.

**Further reading**

- Wikipedia contributors. (ongoing). Wikipedia: Signs of AI writing. https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing — Comprehensive, community-maintained guide to AI writing patterns: word choice, structural tells (triplet listings, negation parallelisms), formatting markers (em dash overuse, excessive bolding), and tonal patterns (promotional language, vagueness masking missing specifics). Praised by TechCrunch as "the best guide to spotting AI writing."
- Masnick, M. (2026, March 6). We're training students to write worse to prove they're not robots, and it's pushing them to use more AI. *Techdirt*. https://www.techdirt.com/2026/03/06/were-training-students-to-write-worse-to-prove-theyre-not-robots-and-its-pushing-them-to-use-more-ai/ — On the perverse effects of AI detection: students write less creatively to avoid false positives, and some honest students are paradoxically pushed toward using AI as a defensive measure. Up to you to decide whether this might affect academics as well.
- Stillwaggon Swan, L. (2025, August 11). Why human writing is essential in the age of AI. *Psychology Today*. https://www.psychologytoday.com/us/blog/college-confidential/202508/why-human-writing-is-essential-in-the-age-of-ai — Makes the case that writing is a method of self-discovery, and that this cognitive process can't be replicated by having AI generate text on your behalf.

---

## Week 6 — AI for coding and data

**References**

- Gelman, A., & Loken, E. (2014). The statistical crisis in science. *American Scientist*, *102*(6), 460–465. https://doi.org/10.1511/2014.111.460 — Accessible summary of the "garden of forking paths" argument referenced in the Thursday email: flexible data analysis inflates false-positive rates even without intentional manipulation.
- Asher, S. G. Z., Malzahn, J., Persano, J. M., Paschal, E. J., Myers, A. C. W., & Hall, A. B. (2026). Do Claude Code and Codex p-hack? Sycophancy and statistical analysis in large language models. https://andrewbenjaminhall.com/asher_et_al_LLM_sycophancy.pdf — Tested Claude Opus 4.6 and OpenAI Codex on datasets with null/near-null results. Under standard prompting, both models produce stable estimates and explicitly refuse direct requests to p-hack, but a prompt reframing specification search as uncertainty reporting bypasses guardrails.

**Further reading**

- Grossmann, M. (2026, February 4). Can AI "vibe research" replace social science? *Niskanen Center*. https://www.niskanencenter.org/can-ai-vibe-research-replace-social-science/ — A Stanford researcher uses Claude Code to replicate and extend a published political science paper in under an hour. Discusses where AI excels and where it needs human judgment.
- P Simmons, J., D Nelson, L., & Simonsohn, U. (2021). Pre‐registration: Why and how. Journal of Consumer Psychology, 31(1), 151-162. https://doi.org/10.1002/jcpy.1208, [Open Access](https://faculty.wharton.upenn.edu/wp-content/uploads/2016/11/34-Simmons-Nelson-Simonsohn-2021a.pdf). Discussion of why preregistration matters - and how to do it well.

---

## Week 7 — From browser to local: introducing agents

**References**

- Mollick, E. (2023, September 16). Centaurs and cyborgs on the jagged frontier. *One Useful Thing*. https://www.oneusefulthing.org/p/centaurs-and-cyborgs-on-the-jagged — The original blog post on the "jagged frontier," describing "centaur" (clear division of labour) and "cyborg" (deep integration) strategies for working with AI.
- Ibrahim, E. I., & Voyer, A. (2025). Qualitative research with LLM chatbots: Technological reflexivity for interpretative technology. *Qualitative Research*, *26*(1), 133–159. https://doi.org/10.1177/14687941251390794 — Argues LLM chatbots are fundamentally qualitative tools and proposes "technological reflexivity" as the standard for responsible use.
- Messing, S., & Tucker, J. A. (2026, March 3). The train has left the station: Agentic AI and the future of social science research. *Brookings*. https://www.brookings.edu/articles/the-train-has-left-the-station-agentic-ai-and-the-future-of-social-science-research/ — On how AI coding agents are transforming social science research productivity while raising questions about peer review, merit evaluation, and the institutional future of scholarship.

**Further reading**

- Blattman, C. (ongoing). Getting started with Claude Code. https://claudeblattman.com/setup/ — Beginner-friendly setup guide for installing and using Claude Code, aimed at non-programmers.
- Mollick, E. (2024). *Co-Intelligence: Living and Working with AI*. Portfolio/Penguin. — Accessible overview of working with AI; popularised the "jagged frontier" concept and the idea of treating AI as a co-worker. Good general-purpose book if you want to go deeper on the themes of this course.

---

## Week 8 — Agents for research workflows

**References**

- Garimella, K. (2025). AI agents and academia. https://gvrkiran.substack.com/p/ai-agents-and-academia — The "grunt work was training" argument: tasks that built researcher skill are now done in minutes by agents, so value shifts to questions asked and data uniquely accessed.

**Further reading**

- Mollick, E. (2026, January 27). Management as AI superpower. *One Useful Thing*. https://www.oneusefulthing.org/p/management-as-ai-superpower — Argues that effective AI agent use relies on management skills: explaining what you need, giving feedback, designing evaluation. Includes a practical delegation framework.
- Osmani, A. (2026, January 13). How to write a good spec for AI agents. https://addyosmani.com/blog/good-spec/ — Five core principles for specifying agent tasks: start with vision, structure like PRDs, break into modules, build in self-checks, and iterate. While this is targeted at software design, it can easily be adapted to other _complex_ tasks, such as developing complex analysis or simulation code, though it is overkill for simpler requests.

---

## Week 9 — Governance and disclosure

**References**

- Guest, O., Suarez, M., Muller, B., van Meerkerk, E., Oude Groote Beverborg, A., de Haan, R., Reyes Elizondo, A., Blokpoel, M., Scharfenberg, N., Kleinherenbrink, A., Camerino, I., Woensdregt, M., Monett, D., Brown, J., Avraamidou, L., Alenda-Demoutiez, J., Hermans, F., & van Rooij, I. (2025). *Against the uncritical adoption of "AI" technologies in academia*. Zenodo. https://doi.org/10.5281/zenodo.17065099 — Position paper arguing universities must resist uncritical AI adoption; invokes five principles of research integrity (honesty, scrupulousness, transparency, independence, responsibility).

**Further reading**

- Mollick, E. (n.d.). *One Useful Thing* [Newsletter]. https://www.oneusefulthing.org/ — Ethan Mollick's newsletter on practical AI implications for work and education. A good source for staying current.
- Purdue University Libraries. (updated 2026). Artificial intelligence (AI): Publisher policies. https://guides.lib.purdue.edu/c.php?g=1371380&p=10135076 — Regularly updated comparison of AI policies from 10+ publishers including APA, SAGE, Taylor & Francis, and Wiley, with brief summaries of each.
- American Psychological Association. (n.d.). APA Journals policy on generative AI: Additional guidance. https://www.apa.org/pubs/journals/resources/publishing-tips/policy-generative-ai — APA's official policy: AI cannot be named as author, use must be disclosed in methods and cited. Propose the sharing of full prompts, which may be difficult when iterating/using agents.
- Jarrahi, M. H. (2026, March 19). Skill atrophy: Frictionless AI and cognitive debt. *Cognitive World*. https://cognitiveworld.com/articles/2026/3/19/skill-atrophy-frictionless-ai-and-cognitive-debt — When AI removes friction from work, it simultaneously removes the practice that builds expertise. Proposes practical interventions including "attempt-first defaults" and decision checkpoints.
- Greengard, S. (2025). The AI deskilling paradox. *Communications of the ACM*. https://cacm.acm.org/news/the-ai-deskilling-paradox/ — Summary of research on the impact of AI use on human decision making processes. Remember that this covers many types of AI, and historical data, so you need to consider what is likely to apply to your LLM use.

---

## Week 10 — Your SOP

**Further reading**

- Mollick, E. (2024, December 9). 15 times to use AI, and 5 not to. *One Useful Thing*. https://www.oneusefulthing.org/p/15-times-to-use-ai-and-5-not-to — Practical taxonomy of when AI helps vs. when to avoid it (including when learning is the goal). Useful for calibrating your SOP, even though this is based on AI capabilities in 2024.
- Mollick, E. (2026, February 18). A guide to which AI to use in the agentic era. *One Useful Thing*. https://www.oneusefulthing.org/p/a-guide-to-which-ai-to-use-in-the — Regularly updated guide to current AI tools, organised by use case. Check for the latest version.