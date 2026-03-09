# AGENTS.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Repository purpose
This repository is a small, markdown-only personal site/profile content repo. There is no application runtime in-tree; the main work here is editing and maintaining content quality and links.

## Canonical files
- `README.md`: Main landing page/profile content and the primary navigation hub.
- `resume.md`: Long-form resume content linked from `README.md`.
- `thenet.md`: Hidden/easter-egg style page linked from the `π` link in `README.md`.

## Development commands
There is currently no configured build, lint, or test framework in this repository (no `package.json`, `Makefile`, `pyproject.toml`, or equivalent).

Commonly useful commands while editing:
- Check working tree:
  - `git --no-pager status`
- Review local changes:
  - `git --no-pager diff`
- List tracked files:
  - `git --no-pager ls-files`

Single-test command: not applicable in the current repository state (no test runner configured).

## Architecture and content flow
- The repository is content-first and flat (top-level markdown files, no source submodules).
- `README.md` is the entry point and links to internal content (`resume.md`, `thenet.md`) plus external project/profile links.
- Most meaningful changes involve keeping cross-file links and narrative consistency intact:
  - If `README.md` link text or structure changes, verify the internal targets (`resume.md`, `thenet.md`) still make sense.
  - If `resume.md` is updated significantly, ensure any summary/positioning statements in `README.md` still align.

## Existing agent/rules files
No `WARP.md`, `CLAUDE.md`, Cursor rules, or Copilot instruction files are currently present in this repository.

## Commit policy
- Never credit AI agents (Warp, Claude, Oz, or others) as authors or co-authors in commits.
- Do not mention agents in commit metadata or commit messages.
- All commits must be signed.
