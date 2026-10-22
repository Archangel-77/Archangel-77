# Working rules for this repository

This repo is a personal GitHub profile README plus an HTML/PDF CV published with GitHub Pages. Every sentence here is a factual claim about a real person applying for junior Python backend/automation roles. Treat accuracy as the primary requirement.

## Facts

- Never invent facts, numbers, dates, prices, release counts, customers, metrics or technologies. If a fact is missing, write a `[BRACKETED PLACEHOLDER]` and list it in the reply.
- Do not add a technology, tool, library or pattern unless it already appears in this repo's content or the user states it.
- The user is the only source of truth. Do not infer capabilities from repository names, badges, commit history or other people's READMEs.
- Prefer omitting a detail over estimating it.

## Identity and framing

- One identity only: Python developer, backend and automation focus. No "ML Engineer", "AI Engineer", "Full-stack Developer", "Senior" or other competing titles.
- The author is not a senior engineer. Never imply seniority, years of experience, team leadership, ownership of other people's systems, or scale that is not stated.
- Never mention education, degrees, bootcamps, courses or student status. Do not imply a completed degree.
- Do not use vague "currently working on X" lines unless the user supplies a concrete one-sentence description.

## Banned language

Remove or rewrite: production-grade, battle-tested, scalable, robust, high-performance, cutting-edge, passionate, seamless, "end to end", "designed, built, and operate", "systems that stay predictable under load and failure", "ownership from architecture through operations", "production-ready", "production-style".

Replace each with a plain, specific, checkable statement.

## AI disclosure

- The About section must mention AI assistance in one plain sentence, without apology and without hiding it, and describe the actual role: specify, review, test, deploy, operate.
- For repositories where AI wrote most of the code, never write "I wrote", "I implemented" or "I engineered". Use neutral wording: "Conductor is a PostgreSQL-backed task queue" or "architecture specified by me; implemented with AI".
- Hutsix is the documented exception: the author wrote the core and the UI; AI assisted with much of the remaining code. Preserve that distinction.
- Do not let the disclosure drift into either downplaying or overstating the author's contribution.

## Technical claims

- Every claim must be one the author could defend in a technical interview.
- When a description names a mechanism, the name must match the code: idempotent writes, `ON CONFLICT` deduplication, exponential backoff (with or without jitter), `SELECT ... FOR UPDATE SKIP LOCKED`, pessimistic locking, at-least-once delivery, dead-letter queue, circuit breaker. If the code was not read, list the term under a confirmation header instead of asserting it.
- Describe private repositories in at most one line, or omit them. Never describe internals of private code.
- Do not state coverage percentages, versions, benchmarks or SLAs unless the user confirms them.

## Style

- Plain English, short sentences, no marketing tone. No emojis.
- Structure, in order: header banner and link badges; name and one-line title; About (3-4 sentences, including the AI disclosure); Projects as `###` headings, each followed by its own diagram; Skills as a three-column table; Contact plus a one-line "open to" statement covering internship, junior and freelance roles.
- Keep total length at or under roughly half of any earlier bloated version. Shorter is better than padded.
- No stack dumps inside project descriptions. Put technologies in Skills.
- Include only skills the author would discuss for 15 minutes. When a tier placement is uncertain, ask or flag it rather than guessing.

### Approved visual treatment

The author asked for a visually scannable profile. These are sanctioned; do not strip them as "decorative":

- One header image: the Hutsix banner from `hutsix-public`, or whatever replaces it.
- At most four link badges in the header, and only for pointing at something real: email, LinkedIn, CV, PyPI. No skill badges, no star/commit/coverage counters, no profile-view counter.
- One Mermaid diagram per flagship project that has a mechanism worth showing. A diagram is a claim: it must match the code, and it must render.
- Skills as a three-column table with headers Solid, Working knowledge, Learning.

Screenshots are allowed only if they show real data and contain no personal information. Do not publish a capture that reads "No data" or that includes browser tabs, bookmarks, file paths or account names.

## Site integrity

- `cv/`, `index.html`, `.nojekyll` and the Pages workflow publish a live CV. Do not rename, move or restructure them, and keep the published CV URL working.
- `generate_resume.py` produces the resume artifacts. Do not touch it unless the task is about the resume.
- Verify every link before finishing. Keep the mailto, LinkedIn and CV links intact unless the user asks otherwise.

## Process

- If a required fact is unknown, ask the user or leave a placeholder. Never guess.
- If a change introduces new claims, list every one of them in the reply for confirmation.
- Do not commit secrets, keys, tokens, customer data or private repository contents.
- Do not reformat, restructure or "improve" parts of the repo unrelated to the request.
- Commit messages use conventional prefixes (`docs:`, `chore:`, `ci:`, `feat:`), matching existing history.
