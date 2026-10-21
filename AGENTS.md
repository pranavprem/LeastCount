# Agent guide

LeastCount is an unimplemented stub. Read this before changing the repo.

## What is here

- Created January 23, 2022 by Pranav Prem (`pranavprem/LeastCount`). One commit until this documentation refresh.
- Original pitch, still the point of the project: a basic Least Count card game so friends who are not in the same place can play each other.
- Tracked files are documentation plus `.gitignore`. There is no source, no tests, no lockfile, and no CI.

Least Count itself is a draw-and-discard card game whose scoring and show rules vary by table. This repo never picked a variant. Do not treat a blog post, an app-store blurb, or your own memory of the game as the spec.

## Architecture

There is none. Do not infer a server, a client, a package layout, or a Python module from the ignore file.

## Conventions

- Keep the original README pitch. It is informal on purpose.
- Do not add a license. That is the owner's decision.
- Do not invent the game, a runtime, dependencies, tests, or CI unless the owner explicitly asks for an implementation. If they do, confirm the rules variant and the stack before writing code. House rules disagree on hand size, jokers, card values, legal shows, and penalties.
- Documentation lives in Markdown. `AGENTS.md` is the agent guide; `CLAUDE.md` only points here. Do not copy this file into `.cursor/rules` or into another guide.
- Never commit secrets, `.env` files, or credential dumps.

## Commands

Nothing to run, lint, or test. There is no dependency install.

```bash
git status
```

That is the useful check: the tree should stay docs and `.gitignore` until an implementation is actually requested.

## Gotchas

- `.gitignore` started as GitHub's Python template from the 2022 initial commit. It is now the current template from [github/gitignore](https://github.com/github/gitignore) `Python.gitignore`, with a short local section at the bottom for OS junk and common credential filenames. Django, Flask, Celery, and the other headings are copied from that template. No framework was selected.
- Upstream stopped ignoring `.python-version` by default (the 2022 file ignored it). If a version file appears later, it is meant to be committed for an application.
- `lib/` is ignored because the Python template says so. Do not put source there.
- Git history has no hardcoded credentials. The scan is the initial commit only. Do not add any.
