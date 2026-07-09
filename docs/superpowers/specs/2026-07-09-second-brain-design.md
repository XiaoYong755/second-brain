# Second Brain Design

**Date:** 2026-07-09

## Goal

Build a local-first second brain that is friendly to Obsidian but not dependent on it, with a Karpathy-style wiki core for LLM knowledge plus space for personal knowledge and project work.

## Design Summary

The system uses a mixed structure:

- `00 Inbox` for quick capture
- `10 Wiki` for long-lived knowledge pages
- `20 Projects` for active work
- `30 Journal` for time-based notes
- `40 Library` for source material notes
- `90 Archive` for inactive material
- `_assets` for attachments

The core idea is that information does not stay as raw notes forever. External material first lands in `Inbox` or `Library`, then the valuable parts are rewritten into `Wiki` pages that represent durable understanding. Projects and journal notes connect knowledge back to real work and real time.

## Top-Level Structure

### `00 Inbox`

The default landing zone for fragmented input:

- fleeting ideas
- copied quotes
- web snippets
- unfinished notes
- thoughts that need sorting

### `10 Wiki`

The long-term knowledge layer. Pages here should be maintained, linked, and compressed over time instead of remaining as raw excerpts.

This is the system center of gravity, especially for LLM-related learning.

### `20 Projects`

A workspace for active projects. Each project gets its own folder and can contain:

- goals
- status
- decisions
- meeting notes
- action lists
- retrospectives

### `30 Journal`

Time-based notes for daily or weekly context. This is where progress, open questions, and evolving thoughts can live without forcing premature structure.

### `40 Library`

Structured notes for outside materials such as:

- papers
- books
- articles
- courses
- talks

Library notes capture source understanding. They are not the same thing as wiki pages.

### `90 Archive`

A parking area for finished, outdated, or no-longer-useful material so the active system stays clean.

### `_assets`

Central storage for images, PDFs, screenshots, and attachments.

## Wiki Structure

`10 Wiki` should contain:

- `Home.md`
- `General/`
- `LLM/`

`10 Wiki/LLM/` should contain:

- `Concepts/`
- `Models/`
- `Papers/`
- `People/`
- `Orgs/`
- `Tools/`
- `Datasets/`
- `Benchmarks/`
- `Systems/`
- `Open Questions/`

### Wiki Principles

- `Concepts` store durable understanding
- `Papers` and `Models` are higher-churn entry points
- useful ideas should eventually be distilled into `Concepts`, `Systems`, or `Open Questions`
- wiki pages should reflect the user's own mental model rather than the source's folder structure

## Naming Rules

- Use English file names where possible
- Prefer short kebab-case for topic pages such as `in-context-learning.md`
- Keep proper names in their standard form such as `Andrej Karpathy.md` or `OpenAI.md`
- Use mixed-language content freely in note bodies
- Avoid date prefixes inside `Wiki`
- Use one topic per page

## Templates

The initial system should include templates for:

- inbox note
- wiki note
- paper note
- project note
- daily note

Each important wiki page should begin with a short `One-line summary`.

## Information Flow

The system should encourage these flows:

- fragmented input -> `00 Inbox`
- source material -> `40 Library`
- durable understanding -> `10 Wiki`
- active execution context -> `20 Projects`
- time context -> `30 Journal`

### Decision Rule

- if it is not processed yet, put it in `Inbox`
- if it is source material, put it in `Library`
- if it is stable understanding, move it into `Wiki`
- if it is tied to active execution, put it in `Projects` or `Journal`

## Navigation

`10 Wiki/Home.md` should provide:

- start points
- core maps
- active work links
- review queues

This page should let the user begin working immediately without hunting for notes.

## Linking Rules

- important concept pages should link to each other
- paper pages should link back to related wiki pages
- project pages should link to supporting knowledge pages
- every durable knowledge page should have a `Related` section

The goal is a navigable map, not maximal backlink density.

## Minimum Viable Version

The first usable version should include:

- the full directory scaffold
- `README.md`
- `10 Wiki/Home.md`
- `10 Wiki/LLM/LLM Index.md`
- the five starter templates
- one example inbox note
- one example paper note
- one example wiki note
- one example project note

## Why This Fits the User Request

This design combines:

- Karpathy-style wiki accumulation for LLM knowledge
- local-first Markdown portability
- inbox capture for low-friction use
- project and journal layers so the system supports real work, not just storage

## Spec Review

This design is intentionally small, local-first, and does not depend on any proprietary application features. There are no unresolved placeholders, and the scope is focused on a first usable second-brain scaffold rather than automation or advanced plugins.
