# AGENTS.md — using Deslopify with any AI coding agent

This file is a short guide for AI coding agents (and the people running them). Deslopify is packaged as a Claude Code plugin, but the skill inside it is written in an open format that several other agents understand too.

## What's in this repo

- `skills/deslopify/` — the skill: a `SKILL.md` (plain instructions) and two reference files (the full trope catalog and its sources). This folder is the portable part.
- `agents/detrope.md` — a Claude Code subagent version of the same editor, so other agents/skills can call it programmatically and receive the cleaned text back. Claude Code-specific; skip it elsewhere.
- Everything else is packaging.

The skill removes AI-writing tells from prose (em-dash abuse, "It's not X — it's Y", "delve", bold-first bullets, hedging clusters, and a few dozen more) while preserving the author's meaning and voice.

## Install, by agent

**Claude Code** — install it as a plugin:

```
/plugin marketplace add axel-pm/deslopify
/plugin install deslopify@deslopify
```

**OpenAI Codex, and other agents that read the open skill format** — copy (or symlink) the skill folder into the place that agent looks for skills. For Codex and several others, that's an `.agents/skills/` folder in your project or home directory:

```sh
git clone https://github.com/axel-pm/deslopify
mkdir -p ~/.agents/skills
cp -R deslopify/skills/deslopify ~/.agents/skills/
```

**Any other agent** — point it at `skills/deslopify/SKILL.md` and tell it to follow the instructions on your draft. It's plain Markdown; nothing is locked to one vendor. Make sure the agent can also read the `references/` folder next to it — that's where the full catalog lives.

## What it needs to run

Nothing. No scripts, no dependencies, no API keys, no network. It's instructions.

## Credit

The trope catalog is based on [tropes.fyi](https://tropes.fyi) by [Ossama](https://ossama.is), extended with the sources listed in `skills/deslopify/references/sources.md`.
