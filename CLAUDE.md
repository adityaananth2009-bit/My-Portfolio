# CV Project — Claude Code Configuration

## Project

Aditya Ananth's CV. Files:
- `Aditya_Ananth_CV_Final.html` — browser/web version
- `Aditya_Ananth_CV_Final.pdf` — 2-page A4 print version
- `CV_Update_Notes (1).txt` — change log for the latest CV update

## Installed Tools & Skills

### impeccable (v3.0.1)
- **Installed:** 2026-06-15
- **Command:** `npx impeccable install` (selected project scope, defaulted to Claude Code + Codex)
- **What it does:** Design skills, slash commands, and anti-pattern detection for AI coding agents
- **Config written to:** `.claude/settings.local.json`, `.agents/`
- **Next step:** Run `/impeccable init` in Claude Code to set up design context

### Emil Kowalski skill (`emil-design-eng`)
- **Installed:** 2026-06-15
- **Command:** `npx skills add emilkowalski/skill`
- **What it does:** Encodes Emil Kowalski's philosophy on UI polish, component design, animation decisions, and invisible details that make software feel great
- **Location:** `.agents/skills/emil-design-eng` (symlinked into `.claude/skills/`)

### Taste skill bundle (Leonxlnx/taste-skill) — 13 skills
- **Installed:** 2026-06-15
- **Command:** `npx skills add Leonxlnx/taste-skill`
- **Skills installed:**
  - `brandkit`
  - `industrial-brutalist-ui`
  - `gpt-taste`
  - `image-to-code`
  - `imagegen-frontend-mobile`
  - `imagegen-frontend-web`
  - `minimalist-ui`
  - `full-output-enforcement`
  - `redesign-existing-projects`
  - `high-end-visual-design`
  - `stitch-design-taste`
  - `design-taste-frontend`
  - `design-taste-frontend-v1`
- **Location:** `.agents/skills/<name>` (each symlinked into `.claude/skills/`)
- **Security:** All 13 passed Gen, Socket, and Snyk checks (Safe / 0 alerts / Low Risk)

## How to Use These Skills

Skills are invoked via slash commands in Claude Code. Examples:
- `/emil-design-eng` — apply Emil Kowalski UI polish principles
- `/high-end-visual-design` — apply high-end visual design taste
- `/minimalist-ui` — apply minimalist UI principles
- `/redesign-existing-projects` — redesign guidance for existing work
- `/impeccable init` — initialise impeccable design context for this project

> Note: Skills run with full agent permissions. Review skill content before use in sensitive contexts.
