# Agent workflow

This repository uses a project memory bank. The checked-in source, tests, and deployment configuration are authoritative; memory notes are a navigation and handover aid.

## Start sequence — every new session and after pulling changes

1. Read `AGENTS.md` (or `CLAUDE.md`), this file, and `memory-bank/toc.md`.
2. Read `memory-bank/activeContext.md`, the latest `memory-bank/tasks/YYYY-MM/README.md`, and the relevant project brief, architecture, and tech notes.
3. Inspect `git status`, recent commits, and the files relevant to the request. Reconcile any memory-bank statement that conflicts with source before relying on it.
4. State the current task, expected outcome, risks, and verification. A read-only question does not require a task document.

## Work sequence

- Search existing files and patterns before adding a file. Extend a suitable file when possible.
- For code or documentation changes, work on a branch and review the diff. Follow the repository's own tests and deployment rules.
- Record decisions and unresolved issues in the memory bank as they arise. Never put credentials, customer exports, or private runtime data there.
- Treat deployment and live data checks separately from passing tests or a successful build.

## Final document and memory update — every change

In the same change as any source, configuration, asset, or documentation edit:

1. Update `memory-bank/activeContext.md` with the current state, completed work, and next action.
2. Add or update a dated `memory-bank/tasks/YYYY-MM/YYMMDD_topic.md` final document. Include objective, changed paths, evidence, tests, deployment or publication status, and open risks.
3. Update that month's `README.md`, plus `progress.md`, `decisions.md`, `systemPatterns.md`, `techContext.md`, or `toc.md` when the corresponding facts changed.
4. For **every new file**, name its path and why existing files could not serve the purpose in the task document. New memory-bank files must also be listed in `toc.md`.

The GitHub memory-bank check requires an active-context update and a dated task document alongside non-memory changes, and checks that new file paths appear in the task document. Keep the final document factual; do not mark tests or live checks complete without evidence.

A Git pull does not execute repository-provided hooks. The root agent files make this sequence available on checkout, and the GitHub check enforces the update contract on pull requests and pushes to main.
