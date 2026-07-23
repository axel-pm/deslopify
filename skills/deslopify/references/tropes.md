# The full trope catalog

Every tell worth scanning for, grouped by category. The base catalog comes from [tropes.fyi](https://tropes.fyi) by Ossama Chahib; sections drawn from other sources are tagged in brackets and listed in [sources.md](sources.md). Everything here is paraphrased, not copied.

A reminder before you use it: a single occurrence of almost anything below is fine. You are hunting repetition, clustering, and density — not individual words.

## 1. Word choice

- **Magic adverbs**: "quietly", "deeply", "fundamentally", "remarkably", "arguably" used to inflate mundane statements. Delete or replace with something concrete.
- **"Delve" & friends**: "delve", "certainly", "utilize" (→ use), "leverage" as a verb, "robust", "streamline", "harness".
- **Grandiose nouns**: "tapestry", "landscape", "paradigm", "synergy", "ecosystem", "framework" where a plain word fits.
- **Copulative avoidance** — the generalized "serves as" dodge: "serves as", "stands as", "functions as", "operates as", "marks", "represents", "boasts", "features" where plain "is"/"are"/"has" works. AI text avoids the verb "to be" like it costs money. [Wikipedia: Signs of AI writing]
- **Academic excess words**: "underscore", "commendable", "meticulous", "intricate", "notable", "realm", "surge", "pivotal", "garner", "showcase", "foster", "align with", "enhance". Statistically over-represented in post-2022 text. [Kobak et al.; Wikipedia]
- **Lazy extremes**: "every", "always", "never", "all" doing imprecise work where "most", "usually", or a number would be honest. [stop-slop]
- **Legalese in web writing**: "aforementioned", "thus", "wherein", "thereof", "herein" in casual prose.
- **Era drift caveat**: the fashionable AI vocabulary changes with each model generation ("delve"/"tapestry" peaked in 2023–24; "fostering"/"showcasing"/"highlighting" came later). Treat word lists as symptoms, not the disease — the underlying patterns below age better. [Wikipedia]

## 2. Sentence structure

- **Negative parallelism** (the #1 tell): "It's not X — it's Y", "not because X, but because Y", "The question isn't X. The question is Y." Rewrite as a direct statement of Y.
- **"Not X. Not Y. Just Z."** dramatic countdowns.
- **"The X? A Y."** self-posed rhetorical questions answered immediately.
- **Anaphora abuse**: repeating the same sentence opening ("They assume… They assume…").
- **Tricolon abuse**: back-to-back rule-of-three patterns.
- **Filler transitions**: "It's worth noting", "It bears mentioning", "Importantly", "Interestingly", "Notably".
- **Superficial "-ing" analyses**: trailing "…highlighting its importance", "…reflecting broader trends", "…underscoring its role". The clause pretends to analyze but adds nothing.
- **False ranges**: "from X to Y" where X and Y aren't on a real spectrum.
- **Elegant variation**: compulsive synonym-swapping to avoid repeating a word ("the company… the firm… the organization… the enterprise" in one paragraph). Humans repeat words; that's fine. [Wikipedia]

## 3. Agency and hedging

[stop-slop; Kernan]

- **False agency / inanimate actors**: "the decision emerges", "the data suggests a shift", "the framework invites us to consider" — sentences where no person does anything. Name who did what.
- **Vague declaratives**: "The reasons are structural." Structural how? Statements that gesture at substance without delivering any. Add the specifics or cut the sentence.
- **Hedging clusters**: "typically", "often", "might be", "can vary depending on", "more often than not" stacked until the text commits to nothing. One hedge is honesty; five is evasion.
- **Distant-narrator voice**: "People think…", "Many believe…", "One might argue…" where a human would write "you" or "I". Near-total absence of first person across a piece is itself a tell.

## 4. Paragraph structure and rhythm

- **Short punchy fragments** as standalone paragraphs for manufactured emphasis ("He published this. Openly. In a book."). Recombine into normal sentences.
- **Listicle in a trench coat**: prose that's secretly a list ("The first… The second… The third…").
- **Metronomic rhythm**: every sentence the same length, three consecutive sentences with matching structure, every paragraph landing on a punchy one-liner. Human rhythm is uneven — vary it. [stop-slop; Kernan]
- **Immediate bullets, no setup**: diving into bullet lists with no narrative lead-in, or answering a prose question with a table. [Kernan]
- **Colon-titles everywhere**: "X: Why Y Matters" headline constructions on every section. [Kernan]
- **Definition-lead openings**: starting with "X refers to…" / "X is a concept that…" when nobody asked for a definition. [Wikipedia]
- **Outline-shaped conclusions**: "Challenges and Future Prospects" sections; "Despite its X, it faces challenges typical of Y" closers that read like a school-report template. [Wikipedia]

## 5. Tone

- **False suspense**: "Here's the kicker", "Here's the thing", "Here's where it gets interesting", "Here's what most people miss".
- **Patronizing analogies**: "Think of it as…", "It's like a…" when unneeded.
- **"Imagine a world where…"** futurism invitations.
- **False vulnerability**: performative "and yes, I'll admit…", "let's be honest" confessions.
- **"The truth is simple"**: asserting something is obvious/clear instead of showing it; "the real story is…".
- **Grandiose stakes inflation**: "will fundamentally reshape everything", "define the next era".
- **Pedagogical voice**: "Let's break this down", "Let's unpack", "Let's explore", "Let's dive in".
- **Vague attributions**: "experts argue", "industry reports suggest", "observers note" with no named source. Either name the source or cut the claim.
- **Invented concept labels**: coined "X paradox / Y trap / Z creep" presented as established terms.
- **Register mismatch**: polished, hard-hitting magazine prose in a context where no human writes that way — a cold email, a commit message, a Slack reply. Match the register the situation actually calls for. [Paul Graham]
- **Canned significance claims**: "has been profiled in national media", "maintains an active social media presence", "solidifying its status as…" — résumé-filler assertions of importance. [Wikipedia]

## 6. Content density

[Shaib et al.; stop-slop; Kernan]

The deepest problem under all the surface tells: **low information density**. Slop is text where little would be lost by deleting it — no numbers, no names, no dates, no sensory detail, no falsifiable claims. If a paragraph could describe a hundred different products or ideas equally well, it says nothing about this one. When rewriting, push toward specifics that are already present in the source material (never invent them); when nothing specific exists, cut the passage rather than re-dressing it.

## 7. Creative-prose slop

For fiction and narrative writing. Statistically over-represented phrases in LLM-generated stories: [slop-forensics / EQ-Bench]

- "a symphony of", "a testament to", "palpable tension", "ethereal glow"
- "barely above a whisper", "eyes glinted", "shivers down the spine", "heart pounding in her chest"
- Watch for over-represented three-word chunks generally — slop lives in stock phrases more than single words.

## 8. Formatting

- **Em-dash addiction**: cut to at most 2–3 in a whole piece; replace with commas, periods, or parentheses.
- **Bold-first bullets**: every list item starting with a **bolded lead**. Remove the bolding unless it's genuinely a definition list.
- **Unicode decoration**: replace → arrows and "smart"/'curly' quotes with plain words and straight quotes (in plain-text contexts).
- **Over-structured documents**: Title Case On Every Heading, skipped heading levels, horizontal rules between every section, emoji as section bullets, tables where two sentences of prose would do. [Wikipedia]

## 9. Chatbot residue (mechanical pass)

Literal artifact strings that survive copy-paste from chatbots. Near-zero false positives — always safe to remove: [Wikipedia]

- `oaicite`, `contentReference`, `turn0search0`-style tokens, `attributableIndex` (ChatGPT)
- `[cite: 1]`, `[span_1][start_span]` (Gemini)
- `grok_render_citation_card_json` (Grok); `ppl-ai-file-upload` (Perplexity); `:::writing` fences
- `utm_source=chatgpt.com` (and similar) in URLs
- Leaked Markdown syntax (`**bold**`, `##`) in contexts that don't render Markdown
- Citation smells worth flagging (in review mode) rather than silently fixing: DOIs/ISBNs that don't resolve, book citations with no page numbers, declared-but-unused references.

## 10. Composition

- **Fractal summaries**: intro-then-recap at every level. Cut redundant summaries.
- **Dead metaphor**: one metaphor beaten 5–10 times. Use it once, then move on.
- **Historical analogy stacking**: rapid-fire "Apple didn't build X. Facebook didn't build Y." lists.
- **One-point dilution**: the same thesis restated ten ways. Cut the repetition down to one clear statement.
- **Content duplication**: verbatim repeated paragraphs/sections. Delete the dupe.
- **Signposted conclusion**: "In conclusion", "To sum up", "In summary". Just end.
- **"Despite its challenges…"**: the acknowledge-then-dismiss formula. Rewrite honestly or cut.
- **Too-perfect surface**: zero typos combined with a voice that doesn't match the author's other writing. You can't fix this by editing, but flag it in review mode. [Kernan]

## Not tells (do not strip)

Wrongly accused features — leave them alone unless they cluster: [Wikipedia "ineffective indicators"]

- The em dash itself, used sparingly and well.
- Smart quotes, correct grammar, clean spelling.
- Ordinary uses of "important", "significant", "notable".
- One rule of three, one rhetorical question, one metaphor, one short punchy sentence.
- Any single item from this catalog, once.
