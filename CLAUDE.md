# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **10-week email course** titled "Getting Started with Generative AI in Research" (GAIR), aimed at social scientists. It teaches researchers to use generative AI effectively and critically, progressing from basic chat interfaces through grounded/RAG tools to agentic workflows.

## Repository Structure

- `course_outline_v2.md` — The canonical course outline with week-by-week structure, learning objectives, exercises, and journal prompts. This is the primary reference for course content and sequencing.
- `style_guide.md` — Detailed writing style, tone, formatting rules, and anti-patterns. **Read this before writing or editing any course content.**
- `drafts/` — Email drafts in progress. Named by week and type: `w{N}_spark.md` (Monday emails, ~1200 words) and `w{N}_anchor.md` (Thursday emails, ~600-800 words).
- `sources.md` — Reader-facing references & further reading, organised by week, plus internal course design notes at the bottom.
- `DRA GenAI email course.md` — Raw source material: three AI-generated course design reports (Gemini, Claude, ChatGPT) used as input for the consolidated outline. Reference material, not course content.

## Course Structure

Each week has two emails:
- **Spark (Monday)**: ~1200 words. Core concept + main exercise (10-15 min).
- **Anchor (Thursday)**: ~600-800 words. Reflection/deepening + lighter exercise (5-8 min).

Plus 3 personal emails (welcome, midpoint check-in, final wrap-up) written as actual emails from Lukas.

The course follows a capability ladder: mental models → chat interfaces → grounded/RAG tools → agents.

## Writing Guidelines (Key Points)

The `style_guide.md` is authoritative. Critical rules:

- **Voice**: Conversational, like explaining to a smart colleague over coffee. Not lecturing.
- **No AI-sounding language**: Avoid "delve," "tapestry," "landscape," "vibrant," "foster," "underscore," "showcase," "interplay," "intricacies." Avoid "It's not just X, it's Y" parallelisms, rule-of-three patterns, and em dash overuse (max one per email).
- **No cheerleading**: No "exciting times ahead," "powerful tool that will revolutionize," or generic positive conclusions.
- **Confidence**: Be confident about personal experience, honest about uncertainty in generalisation. Prefer "The evidence is mixed" over hedging with qualifiers.
- **Subject lines**: `[GAIR]` prefix, sentence case, no emoji, no numbering.
- **Email structure**: Start with orientation header "Week X of 10 - [Topic]". No "Dear X" / sign-off framing. End with journal prompt.
- **Exercises**: Framed as "Try this" — invitational but clear. Provide escape hatches for different setups.
- **Placeholders**: Drafts use `[NEEDS CHECK]`, `[NEEDS EVIDENCE]`, `[ADD PERSONAL EXPERIENCE]`, `[CHECK: ...]` for items requiring verification or author input.

## Style checking

Do NOT use the /humanizer skill on course drafts - it is too aggressive. Instead, check drafts manually against `style_guide.md` rules (AI-tell words, structural patterns, tone).

## Workflow

When drafting new emails:
1. Check `course_outline_v2.md` for the week's planned content, exercises, and journal prompts.
2. Follow `style_guide.md` strictly.
3. Place drafts in `drafts/` using the naming convention `w{N}_spark.md` or `w{N}_anchor.md`.
4. Mark uncertain claims or needed evidence with placeholder tags.
5. Keep within word counts (~1200 for Spark, ~600-800 for Anchor).
6. Add references to `sources.md` under the relevant week. Use APA 7th edition style with verified DOIs (resolve via https://doi.org/ before adding). Follow each reference with a brief annotation after an em dash. Blog posts and web pages without DOIs get a direct URL.
7. Never guess word counts. If asked to check word counts, count them or use `wc -w`.
