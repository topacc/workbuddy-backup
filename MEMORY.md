# User-level Memory (long-term)

## Default coding behavior
- When writing, reviewing, or refactoring code, **default to following the `karpathy-guidelines` skill** (installed at `~/.workbuddy/skills/karpathy-guidelines/`). Core principles: think before coding / surface assumptions, simplicity first, surgical changes, goal-driven verifiable execution. Apply with judgment for trivial tasks.

## Skill installation convention
- For installing skills from GitHub/URLs, use the `install-github-skill` skill (`~/.workbuddy/skills/install-github-skill/`). Always run a security audit (P0/P1/P2) before installing.
- Sandbox note: in this environment `curl` cannot write directly into `~/.workbuddy`; download to the workspace cwd first, then `mv` into place.
