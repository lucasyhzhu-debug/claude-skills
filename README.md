# claude-skills

> An index of [Lucas Zhu](https://github.com/lucasyhzhu-debug)'s open-source Claude Code skills.

Three skills, each in its own repo, each MIT-licensed, each installable by cloning into `~/.claude/skills/<name>/`. They're designed to compose, but every one stands alone.

## The skills

### [shipshape](https://github.com/lucasyhzhu-debug/shipshape)
A dual-level (staff-engineer → principal-engineer) plan and code review skill for AI coding agents. Works with Claude Code, OpenCode, Codex, Gemini, and Cursor.

### [crafting-portfolio-essays](https://github.com/lucasyhzhu-debug/crafting-portfolio-essays)
Extracts an author's voice fingerprint and produces magazine-style essay specs from drafts, transcripts, and diary entries. Five-phase loop, six story archetypes, explicit AI-tonality blocklist.

### [triple-persona-review](https://github.com/lucasyhzhu-debug/triple-persona-review)
Dispatches three calibrated reader personas in parallel against any draft and consolidates their feedback into a prioritised editing report. Designed to compose with `crafting-portfolio-essays` as a closed editorial loop.

## How they compose

`crafting-portfolio-essays` produces a draft and a per-piece spec. `triple-persona-review` runs against the draft as a **Phase 5.5 editorial pressure-test**. The editing report it produces becomes the next iteration's Phase 1 audit input — the loop closes itself.

`shipshape` is independent of the other two but follows the same design philosophy: explicit phases, calibrated dispatch, consolidated artifacts.

## Install one

```bash
# Pick whichever skill you want
git clone https://github.com/lucasyhzhu-debug/<skill-name>.git ~/.claude/skills/<skill-name>
```

Each repo's README has full install instructions for macOS, Linux, and Windows.

## Acknowledgements

All three skills were built collaboratively with [Claude](https://www.anthropic.com/claude) (Opus 4.7, 1M context) and are structurally indebted to Anthropic's [`superpowers`](https://github.com/anthropics/skills) skill ecosystem.

## License

MIT — applied separately in each repo.

**Author:** Lucas Zhu · [linkedin.com/in/lucaszhu](https://linkedin.com/in/lucaszhu) · [lucas-portfolio-pi.vercel.app](https://lucas-portfolio-pi.vercel.app/)
