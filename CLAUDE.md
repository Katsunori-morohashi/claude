# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a **public previews repository** used to host temporary public previews of AI prototypes. It is intentionally minimal: as of the latest commit it contains only this file and `README.md`, with no application code, build system, tests, or CI configured yet.

## Current Structure

```
.
├── README.md   # One-line description of the repository's purpose
└── CLAUDE.md   # This file
```

## Development Workflow

- **Branching**: `main` is the default branch. Do development on feature branches (the convention in use is `claude/<topic>-<id>` for Claude Code sessions) and push with `git push -u origin <branch-name>`.
- **No build/test/lint commands exist yet.** There is no `package.json`, `Makefile`, or other tooling. If you add a prototype that needs tooling, add the relevant commands to this file at the same time.

## Key Conventions

- **Prototypes are temporary and public.** Anything committed here should be treated as publicly visible. Never commit secrets, API keys, credentials, or private data.
- **Keep prototypes self-contained.** Each preview/prototype should live in its own top-level directory with its own README explaining what it is and how to run it, so it can be added or removed independently.
- **Update this file as the repo grows.** When a prototype introduces a language, framework, or command set, document the essentials (setup, run, test commands) here so future sessions don't have to rediscover them.
