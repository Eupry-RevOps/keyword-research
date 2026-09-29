# System patterns — AI Keyword Research

## Current architecture

FastAPI routes coordinate DataForSEO collection, relevance and strategy analysis through Anthropic, and local SQLite job history. Google OAuth restricts access.

## Invariant

Do not present development or deployment status as proof that external SEO data and AI outputs were verified live.

## Change rule

Search existing implementation and documentation before creating a file. Record the chosen extension point or the reason a new file is needed in the final task document. Update this file when an architectural pattern actually changes.

Sources: README.md; DEPLOY.md.
