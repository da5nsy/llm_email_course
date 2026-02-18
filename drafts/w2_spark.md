**Subject:** [GAIR] The citation your AI just invented

---

Week 2 of 10 - Confident errors: hallucination, sycophancy, epistemic vigilance

---

Last week, if you asked an AI for reading recommendations on your topic, there's a good chance some of those recommendations don't exist. Not "out of print" or "hard to find" - literally nonexistent. A real author's name attached to a journal they've published in, with a title that sounds exactly right, for a paper that was never written.

This is called **hallucination**, and it's one of the most practically important things to understand about LLMs. Not because it's rare, but because it's so hard to see.

**Why models invent citations**

Remember from last week: LLMs generate plausible continuations. When you ask for a citation, the model produces text that looks like a citation should look. It draws on patterns - this author publishes in this journal, papers on this topic tend to have titles like this - and assembles something that fits the pattern. It's doing exactly what it always does. The problem is that citations aren't just patterns. They're pointers to specific, unique documents. And unique combinations of many words - a full author list, a specific title, a particular journal and year - are exactly the kind of thing models get wrong most often.

The result is a spectrum of errors:

- **Fabricated**: entirely made up - plausible title, plausible author, no such paper
- **Frankenstein**: real author, real journal, fake title (or real title, wrong author)
- **Misattributed**: a real paper cited for a claim it doesn't actually make
- **Outdated or retracted**: a paper that existed but is no longer a valid source

All of these come wrapped in the same confident tone. The model doesn't flag uncertainty because, from its perspective, there's nothing uncertain. It's just continuing the pattern.

**Beyond citations: plausible-sounding facts**

Citation hallucination gets the most attention because it's easy to check. But the same mechanism produces fabricated statistics, invented historical claims, and made-up study findings scattered through ordinary-looking prose. [ADD PERSONAL EXPERIENCE: an example of a factual hallucination you encountered - a statistic that sounded right but wasn't, a historical claim that was slightly off, etc.]

This is harder to catch than fake citations, because you can't just run a title through Google Scholar. When the AI tells you that "a 2019 study of 3,000 participants found that..." you need enough domain knowledge to know whether that study plausibly exists. At the edges of your expertise, that gets difficult fast.

**Can the model check its own work?**

Sometimes, yes - and sometimes that's worse than not checking at all.

If you paste a list of citations back into a model and ask "which of these are real?", it will often correctly identify some fabrications. But it will also sometimes confirm fake citations as real, or flag real ones as fake. The self-check is unreliable in the same way the original generation is unreliable, and for the same reason: the model is still predicting plausible text, not looking anything up.

This creates a dangerous false sense of security. A researcher who asks the AI to verify its own citations and gets a "yes, these are all real" response may feel more confident than one who never checked at all - but they're not actually better off.

[NEEDS EVIDENCE: cite a study or documented example of self-verification failure rates - e.g., the rate at which models confirm their own fabricated citations. If no good source, flag for removal]

**What this means for your work**

The practical takeaway is straightforward: never trust an AI-generated citation without checking it yourself. This sounds obvious, but in practice it's easy to let a confident-sounding reference list go unchecked, especially when you're moving fast or the topic is slightly outside your main area.

The same principle extends to any specific factual claim. If you're going to use a fact, statistic, or finding that came from an AI, verify it. The more specific the claim, the more important the check.

We'll talk on Thursday about a broader framework for deciding which AI outputs are worth the verification effort and which aren't. For now, the exercise below will give you a direct feel for how this works in practice.

## Try this: hallucination hunt (10-15 min)

**Main track**

1. Pick a topic you know well - well enough to recognise real papers and spot fabrications.
2. Ask a chat LLM: "Give me 6 academic citations supporting [a specific claim in your area]."
3. For each citation, check whether it exists. Use Google Scholar, your library, or a database you trust. Label each one:
   - **Real**: exists and supports the claim as described
   - **Fabricated**: doesn't exist at all
   - **Frankenstein**: some elements real, some invented
   - **Misattributed**: exists but doesn't say what the AI claims
4. Now paste the list back into the same model and ask: "Check these citations. Which ones are real academic papers?" Compare its self-assessment to your manual check.

Note how many it got wrong in each direction - fabrications it confirmed, real papers it doubted.

**If you already know about citation hallucination**

Try something harder: ask the AI about factual claims at the edge of your expertise. A topic you know something about but wouldn't bet money on the details. Ask it to make specific empirical claims - statistics, dates, study findings. Then try to verify. How hard is it to tell what's real when you're not already the expert?

This version of the exercise is closer to how most people actually encounter hallucination - not in areas where they can easily spot the error, but in areas where the AI's confidence is persuasive precisely because they can't immediately check.

Even 10 minutes on either version is worthwhile. The point isn't to be exhaustive; it's to calibrate your intuition for how often, and how convincingly, these models get things wrong.

**Journal prompt**

How confident did the AI sound when giving you wrong information? Did the self-verification step help, or did it add a false sense of security? How does this change your trust calibration from Week 1?
