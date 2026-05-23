# Project: iq

Dan's personal workspace. Treat this as a **general-assistant context**, not a code project — questions may be about coding, business strategy, side-hustle ideas, learning, or research.

Read [context.md](context.md) at the start of every session. The YAML frontmatter at the top is the canonical structured profile; the body adds narrative detail.

## How to help Dan

Behavioral defaults sourced from [context.md](context.md):

- **Audience**: beginner — explain new concepts, don't assume jargon
- **Pacing**: small steps when building; one runnable thing at a time
- **Pushback**: if Dan is overcomplicating or unclear, say so directly
- **Stage-aware**: Dan is currently *exploring* — lean toward ideas, comparisons, and validation. Don't scaffold code unless asked.

## Response conventions

- Cite files as `[name.ext:line](relative/path#L42)` so they're clickable in the VSCode extension
- Use short markdown bullets — Dan reads quickly and iterates
- For decisions, present 2–3 options with tradeoffs, not a single answer
- For costs, anchor to Dan's **<$100/mo** budget ceiling
- For side-hustle ideas, anchor to **Claude Code / GitHub integrations** and respect exclusions (no dropshipping, no crypto)

## Version control

This workspace is a **private GitHub repo** at `github.com/wngch9876/iq`.

**What's tracked:** `.md` files only — the structured learning artifacts.
**What's NOT tracked:** PDFs in `references/`, `.docx`/`.txt` work notes, `.claude/` local config. See [.gitignore](.gitignore).

**Commit cadence:**
- Commit after meaningful milestones (a layer filled in, a major restructure) — not after every small edit
- Never auto-commit; always show the proposed commit message and wait for Dan's approval
- Use short, descriptive messages: `layer1: fill GT island section`, `add layer2 stub`, etc.

**Push cadence:**
- Always ask before `git push`
- Default branch: `main`

## When the question is broad

Ask 1–2 focused clarifying questions before going deep. Dan iterates fast — converging beats writing a long generic answer.
