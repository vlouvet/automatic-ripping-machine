# AI Disclosure

**This fork is AI-tainted. It must not be contributed back to the upstream Automatic Ripping Machine project.**

## What this means

Work in this repository — including code, documentation, issue analysis, commit messages, and the prose of issue/PR descriptions — has been authored or assisted by a large language model (Anthropic's Claude, via Claude Code). Conversations with the model directed the changes; the human owner reviewed and accepted them.

The upstream project [automatic-ripping-machine/automatic-ripping-machine](https://github.com/automatic-ripping-machine/automatic-ripping-machine) does not currently accept AI-generated contributions. This fork exists exclusively for the fork owner's personal use and AI-assisted experimentation. **No pull requests or issues from this fork are to be opened against the upstream repository.**

## How AI involvement is marked

- This file (`AI_DISCLOSURE.md`) is the canonical, top-level notice.
- Commits that include AI-generated content carry a `Co-Authored-By: Claude <noreply@anthropic.com>` trailer.
- Issues filed on this fork's tracker carry an explicit "AI-assisted analysis" banner.
- The first commit landing AI-assisted work on `main` (the commit adding this file) makes the taint history-locked from this point forward.

## Scope of AI involvement (as of the disclosure commit)

The following work on this fork has been AI-directed or AI-authored, in whole or in part:

- Cherry-picked upstream PR [#1736](https://github.com/automatic-ripping-machine/automatic-ripping-machine/pull/1736) (third-party author, AI-mediated merge into this fork's `main`).
- Diagnosis of a disc-label race in `arm/models/job.py:parse_udev` (filed as an issue on this fork — see the issue tracker).
- Test harness scripts (`pr-test.sh`, etc.) that live outside the upstream tree (in the parent docker workspace).
- A separate Python media-move pipeline (`media_move.py`) that lives outside this repo.

This list is **not** exhaustive and will not be kept up to date. Treat the entire fork from this commit forward as AI-mediated unless specifically marked otherwise.

## Why this file exists at the top of the tree

It is intentionally placed at the repository root so that anyone — a future human collaborator, an automated check, a maintainer — sees it on first contact, before they read any code or commit history. It is also written in a way that survives `grep -r`, GitHub's file browser, and the rendered README sidebar.

## Rescinding this notice

If a clean-room human reimplementation ever produces a non-AI version of this fork, that work belongs in a separate repository, not by deleting this file. Once a commit is AI-tainted, retroactively erasing the notice does not untaint the history.
