**Subject:** [GAIR] The citation your AI just invented

---

Week 2 of 10 - Confident errors: hallucination, sycophancy, and the need to stay vigilant

---

Last week, you might have asked an AI for reading recommendations on your topic. If you did, there's a good chance some of those recommendations don't exist. Not "out of print" or "hard to find" - literally nonexistent. A real author's name attached to a journal they've published in, with a title that sounds exactly right, for a paper that was never written.

This is called **hallucination**, and it's one of the most practically important things to understand about LLMs. Even though this has become a lot better over recent years, hallucinations still occur, and can be tough to spot.

**Why models invent citations**

Remember from last week: LLMs generate plausible continuations. When you ask for a citation, the model produces text that looks like a citation should look. It draws on patterns - this author publishes in this journal, papers on this topic tend to have titles like this - and assembles something that fits the pattern. It's doing exactly what it always does. The problem is that citations aren't just patterns. They're pointers to specific, unique documents. And unique combinations of many words - a full author list, a specific title, a particular journal and year - are exactly the kind of thing models get wrong most often.

The result is a spectrum of errors: sometimes references are entirely fabricated, sometimes they are nearly right, sometimes they are even correct, but do not support the claim that the model attributed to them. All of these come wrapped in the same confident tone. The model doesn't flag uncertainty because, from its perspective, there's nothing uncertain. It's just continuing a highly plausible pattern.

**Beyond citations: plausible-sounding facts**

Citation hallucination gets the most attention because it's easy to check, and because there are few other explanations why citations to non-existent papers suddenly started to appear across the academic literature after ChatGPT came out. But the same mechanism produces fabricated statistics, invented historical claims, and made-up study findings scattered through ordinary-looking prose. This can make working with LLMs very frustrating. They can often get a lot of details right, but some details wrong. They are great at reformatting reference lists, but I recently came close to shouting at a model that helpfully decided to fill in all gaps with "plausible" page numbers and DOIs.

**Can the model check its own work?**

Sometimes, yes - and sometimes that's worse than not checking at all.

If you paste a list of citations back into a model and ask "which of these are real?", it will often correctly identify some fabrications. But it will also sometimes confirm fake citations as real, or flag real ones as fake. The self-check is unreliable in the same way the original generation is unreliable, and for the same reason: the model is still predicting plausible text, not looking anything up. The only reliable self-check will catch inconsistencies in the text you provide (e.g. between journal name and DOI).

This creates a dangerous false sense of security. A researcher who asks the AI to verify its own citations and gets a "yes, these are all real" response may feel more confident than one who never checked at all - but they're not actually better off.

However, note that there is a difference when it comes to models that can use tools. Most models can now search the web, which makes self-checking work better. Some models can directly write and execute code that, for instance, checks with Crossref whether DOIs match citations. We'll come back to this in the coming weeks.

**What this means for our work**

Unfortunately, this means that responses from chat interfaces - whether they are citations or factual claims - can never be fully trusted. This sounds obvious, but in practice it's easy to let a confident-sounding claim go unchecked, especially when you're moving fast or the topic is slightly outside your main area. At times, this might also be okay. I regularly ask LLMs for cooking advice - I wouldn't trust one on whether a mushroom is safe to eat, but I appreciate a confident opinion on whether hoisin or toban djan sauce works better for a given dish. Similarly, when I'm torn between two approaches to a statistical problem, I appreciate a pointer even if it might sometimes lead me astray.

Nevertheless, for any specific factual claim, we need to calibrate our confidence. LLMs - like any source - can be useful even if they are sometimes wrong. But unlike humans, they are very poor at telling us how confident they are.

So we need to learn when to become suspicious, and be mindful never to present LLM outputs as "the truth" without adequate verification. I'll share some more thoughts on that on Thursday. For now, the exercise below will give you a direct feel for how this works in practice.

## Try this: hallucination hunt (10-15 min)

**Main track**

1. Pick a topic you know well - well enough to recognise real papers and spot fabrications.
2. Ask a chat LLM: "Give me 6 academic citations supporting [a specific claim in your area]."
3. For each citation, check whether it exists. Use Google Scholar, your library, or a database you trust. Label each one:
   - **Real**: exists and supports the claim as described
   - **Fabricated**: doesn't exist at all
   - **Frankenstein**: some elements real, some invented
   - **Misattributed**: exists but doesn't say what the AI claims
4. Now paste the list back into a new chat with the same model and ask: "Check these citations. Which ones are real academic papers?" Compare its self-assessment to your manual check.

Note how many it got wrong in each direction - fabrications it confirmed, real papers it doubted.

**Or alternatively, if you already spotted hallucinated citations**

Try something harder: ask the AI about factual claims at the edge of your expertise. A topic you know something about but wouldn't bet money on the details. Ask it to make specific empirical claims - statistics, dates, study findings. Then try to verify. How hard is it to tell what's real when you're not already the expert?

This version of the exercise is closer to how most people actually encounter hallucination - not in areas where they can easily spot the error, but in areas where the AI's confidence is persuasive precisely because they can't immediately check.

Spending some time on either version is worthwhile. A key skill in using AI effectively is calibrating your intuition for how often, and how convincingly, these models get things wrong - and starting to learn *when* this might be particularly likely.

**Journal prompt**

How confident did the AI sound when giving you wrong information (if you managed to get wrong information)? Did the self-verification step help, or did it add a false sense of security? Does this exercise change how you approach AI output?
