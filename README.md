# claude-skills

> An index of my open-source Claude Code skills. MIT-licensed. Install by cloning into `~/.claude/skills/`.

## The skills

### [shipshape](https://github.com/lucasyhzhu-debug/shipshape)

Dual-level plan and code review for AI coding agents — a staff-engineer pass, then a principal-engineer pass. Works with Claude Code, OpenCode, Codex, Gemini, and Cursor.

### [crafting-portfolio-essays](https://github.com/lucasyhzhu-debug/crafting-portfolio-essays)

A skill for writing essays in your voice, not the model's. It asks for samples of how you actually write and talk, then builds a tone-and-soul reference plus a per-piece spec.

### [fresh](https://github.com/lucasyhzhu-debug/fresh)

Fire a prompt the moment your next 5-hour usage window resets — full quota for your biggest runs. Same-session or fresh headless session (`--clear`). Windows-first.

### [triple-persona-review](https://github.com/lucasyhzhu-debug/triple-persona-review)

Three readers who don't agree, dispatched in parallel, then consolidated. Built to compose with `crafting-portfolio-essays` as the editorial pressure-test phase.

## How they compose

`crafting-portfolio-essays` produces a draft and a per-piece spec. Run `triple-persona-review` against the draft. Its editing report feeds into the next iteration's audit. The loop closes itself.

`shipshape` is independent — same design philosophy (explicit phases, calibrated dispatch, consolidated artifacts) but for code, not prose. `fresh` is the odd one out: a small scheduling utility that makes the others cheaper to run — queue the heavy loops to start on a full quota window.

## Install one

```bash
git clone https://github.com/lucasyhzhu-debug/<skill-name>.git ~/.claude/skills/<skill-name>
```

Each repo has install instructions for macOS, Linux, and Windows.

## Acknowledgements

All of these were built collaboratively with Claude (Opus 4.7). Indebted to Anthropic's [`superpowers`](https://github.com/anthropics/skills) skill ecosystem.

## License

MIT, applied separately per repo.

Lucas Zhu · [linkedin.com/in/lucaszhu](https://linkedin.com/in/lucaszhu) · [lucas-portfolio-pi.vercel.app](https://lucas-portfolio-pi.vercel.app/)
