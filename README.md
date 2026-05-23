# skills

Personal collection of agent-skills created by me.

These skills are packaged as `SKILL.md`-based capabilities for AI coding agents and are intended to be installable through the `skills.sh` ecosystem.

## About `skills.sh`

[`skills.sh`](https://www.skills.sh/) is Vercel's open directory for agent skills. According to the official docs, skills are reusable capabilities for AI agents, can be installed with `npx skills add <owner>/<repo>`, and are supported across agents including Claude Code, Cursor, Codex, GitHub Copilot, Windsurf, Gemini, and Cline.

## Repository goal

This repo is where I keep my custom agent-skills:

- focused on repeatable workflows
- backed by runnable helper scripts when plain instructions are not enough
- structured so they can be installed and reused instead of rewritten in every session

## Current skills

### `vercel-delete-deployments`

Delete Vercel deployments by status, ID range, or one-off cleanup. This skill includes helper scripts for safer bulk deletion workflows instead of relying on fragile terminal filtering.

Path: `vercel-delete-deployments/`

## Install pattern

After this repo is published on GitHub, the standard `skills.sh` install pattern will be:

```bash
npx skills add aykansal/skills --skill vercel-delete-deployments
```

Replace `<owner>` with the GitHub username or org that hosts this repository.

## Structure

```text
skills/
├─ README.md
└─ vercel-delete-deployments/
   ├─ SKILL.md
   └─ scripts/
```

## Notes

- Each skill should stay self-contained with its own instructions, scripts, and safety guidance.
- Repo-level documentation should explain discovery and installation; skill-level documentation should explain execution details.
