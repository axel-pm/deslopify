# Deslopify

**Paste in a draft (or point at a file). It strips the AI tells — the em-dash pileups, the "It's not X, it's Y" reframes, the "delve"s, the bold-first bullets — and hands back prose that reads like you wrote it.** No scripts, no API keys: it's a plain-Markdown skill for your AI coding agent.

## What problem this solves

AI-drafted text has a fingerprint. Readers have learned it, and once they spot it they stop trusting the words. The fingerprint is a few dozen recurring tropes rather than any one bad word: negative parallelism, tricolons, hedging clusters, fake suspense, metronomic rhythm, "In conclusion".

Deslopify gives your agent a curated, sourced catalog of those tropes and a disciplined way to remove them: rewrite rather than delete, preserve the author's meaning and voice, and never over-correct (one em dash is style; fourteen are a tell).

Two ways to use it:

- **The `deslopify` skill** — say "deslopify this draft" (or "de-slop", "remove the AI tells", "make this sound less like AI"). Works on pasted text or files, in rewrite mode (returns cleaned text plus a change list) or review mode ("flag what's wrong" returns findings without touching the text).
- **The `detrope` subagent** — other agents and skills can call it programmatically and get the cleaned text back. Useful inside writing pipelines.

## Install

**Claude Code** (one command each):

```
/plugin marketplace add axel-pm/deslopify
/plugin install deslopify@deslopify
```

Then just ask, in plain words:

> "Deslopify this: [your draft]"
> "Review draft.md for AI tells — don't rewrite it yet."

**Manual install** (no plugin system): copy `skills/deslopify/` into `~/.claude/skills/` and, optionally, `agents/detrope.md` into `~/.claude/agents/`.

**Using a different agent** (Rovo Dev CLI, Codex, Cursor, …)? See [AGENTS.md](AGENTS.md). The skill is plain Markdown in an open format that several other coding agents read.

## What's in the catalog

- `skills/deslopify/SKILL.md` — the editor's job: modes, method, guardrails, and the core trope list.
- `skills/deslopify/references/tropes.md` — the full catalog: word choice, sentence structure, agency and hedging, rhythm, tone, content density, creative-prose slop, formatting, chatbot residue strings, and composition — plus a "not tells" list so it never strips legitimate human style.
- `skills/deslopify/references/sources.md` — where every section comes from, with licenses.

## A note on trust

This plugin is prose-only: no scripts, nothing executes. It's Markdown instructions your agent reads. MIT licensed; read every file before installing if you like, it won't take long.

## Credits

The heart of this project is the trope catalog from **[tropes.fyi](https://tropes.fyi)** by **[Ossama Chahib](https://ossama.is)** — the clearest, best-curated taxonomy of AI writing tells around. Thank you, Ossama.

The extended catalog also draws on (all paraphrased, licenses noted in [sources.md](skills/deslopify/references/sources.md)):

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) by WikiProject AI Cleanup (CC BY-SA 4.0)
- [stop-slop](https://github.com/hardikpandya/stop-slop) by Hardik Pandya (MIT)
- [slop-forensics](https://github.com/sam-paech/slop-forensics) and the [EQ-Bench slop score](https://eqbench.com/slop-score.html) by Sam Paech (MIT)
- [Kobak et al., *Delving into LLM-assisted writing*](https://www.science.org/doi/10.1126/sciadv.adt3813) (Science Advances, CC BY)
- [Shaib et al., *Measuring AI "Slop" in Text*](https://arxiv.org/abs/2509.19163)
- [Pangram Labs' AI-phrase research](https://www.pangram.com/resources/most-common-ai-phrases), [Sean Kernan](https://seanjkernan.substack.com/p/13-signs-you-used-chatgpt-to-write), Paul Graham's "delve" observations, and [awesome-slop](https://github.com/hwajongpark/awesome-slop) (CC0)

Related work: [skill-deslop](https://github.com/stephenturner/skill-deslop) by Stephen Turner, an independent skill with a scoring-rubric approach.

## Contributing

Issues and PRs welcome, especially new tells with sources, and false positives for the "not tells" list. `claude plugin validate .` checks the manifests.

## License

[MIT](LICENSE).
