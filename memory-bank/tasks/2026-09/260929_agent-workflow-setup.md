# 260929_agent-workflow-setup

## Objective

Add a project-specific start sequence, final task document pattern, memory-bank update contract, and GitHub check to AI Keyword Research.

## Source and reuse analysis

Reviewed README.md; DEPLOY.md and the existing root files. No checked-in memory-bank workflow or equivalent root agent contract covered all three requirements. Existing project documentation is retained and linked. The new files establish the missing persistent process; README.md is extended in place.

## Changed paths and purpose

- `AGENTS.md` — provides the root agent workflow entry or process.
- `CLAUDE.md` — provides the root agent workflow entry or process.
- `WORKFLOW.md` — provides the root agent workflow entry or process.
- `README.md` — links the workflow from the existing project guide.
- `.github/workflows/memory-bank.yml` — checks future documentation updates.
- `memory-bank/README.md` — records project context or task completion.
- `memory-bank/toc.md` — records project context or task completion.
- `memory-bank/projectbrief.md` — records project context or task completion.
- `memory-bank/systemPatterns.md` — records project context or task completion.
- `memory-bank/techContext.md` — records project context or task completion.
- `memory-bank/activeContext.md` — records project context or task completion.
- `memory-bank/progress.md` — records project context or task completion.
- `memory-bank/decisions.md` — records project context or task completion.
- `memory-bank/quick-start.md` — records project context or task completion.
- `memory-bank/tasks/2026-09/README.md` — records project context or task completion.
- `memory-bank/tasks/2026-09/260929_agent-workflow-setup.md` — records project context or task completion.

## Verification and publication

The files are documentation and CI configuration; application runtime code is unchanged. Source facts were taken from README.md; DEPLOY.md. The GitHub check must pass on the pull request before merge. A passing check does not establish live application health.

## Open risks

Git itself does not execute checked-in instructions on pull. Agents must read the root entry files at session start; GitHub checks enforce documentation on reviewed changes, while repository branch protection determines whether a check can block every merge.
