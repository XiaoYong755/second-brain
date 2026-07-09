# Second Brain Scaffold Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a local-first Markdown second-brain scaffold with a Karpathy-style LLM wiki core, starter templates, and example notes.

**Architecture:** Create a clear folder hierarchy with durable knowledge separated from source notes and active project context. Seed the workspace with a homepage, core LLM index, reusable note templates, and a handful of example notes so the system is immediately usable.

**Tech Stack:** Markdown, local filesystem

---

## File Structure

- Create: `README.md`
- Create: `00 Inbox/`
- Create: `10 Wiki/`
- Create: `10 Wiki/Home.md`
- Create: `10 Wiki/General/`
- Create: `10 Wiki/LLM/`
- Create: `10 Wiki/LLM/LLM Index.md`
- Create: `10 Wiki/LLM/Concepts/`
- Create: `10 Wiki/LLM/Models/`
- Create: `10 Wiki/LLM/Papers/`
- Create: `10 Wiki/LLM/People/`
- Create: `10 Wiki/LLM/Orgs/`
- Create: `10 Wiki/LLM/Tools/`
- Create: `10 Wiki/LLM/Datasets/`
- Create: `10 Wiki/LLM/Benchmarks/`
- Create: `10 Wiki/LLM/Systems/`
- Create: `10 Wiki/LLM/Open Questions/`
- Create: `20 Projects/`
- Create: `30 Journal/`
- Create: `40 Library/`
- Create: `40 Library/Papers/`
- Create: `40 Library/Books/`
- Create: `40 Library/Articles/`
- Create: `40 Library/Courses/`
- Create: `90 Archive/`
- Create: `_assets/`
- Create: `_templates/`
- Create: `_templates/inbox-note.md`
- Create: `_templates/wiki-note.md`
- Create: `_templates/paper-note.md`
- Create: `_templates/project-note.md`
- Create: `_templates/daily-note.md`
- Create: `00 Inbox/2026-07-09-welcome-capture.md`
- Create: `10 Wiki/LLM/Concepts/in-context-learning.md`
- Create: `40 Library/Papers/attention-is-all-you-need.md`
- Create: `20 Projects/second-brain-bootstrap/project.md`

### Task 1: Create the directory scaffold

**Files:**
- Create: top-level folders and LLM subfolders listed above

- [ ] **Step 1: Create the folders**

Create the listed directories so the workspace has a stable home for capture, durable knowledge, projects, journal notes, source materials, templates, and assets.

- [ ] **Step 2: Verify the structure exists**

List the folder tree and confirm each planned directory is present.

### Task 2: Write the repository guide and navigation pages

**Files:**
- Create: `README.md`
- Create: `10 Wiki/Home.md`
- Create: `10 Wiki/LLM/LLM Index.md`

- [ ] **Step 1: Write `README.md`**

Document:

- what this repository is for
- the role of each top-level folder
- the simple flow from Inbox or Library into Wiki
- a short “how to start today” checklist

- [ ] **Step 2: Write `10 Wiki/Home.md`**

Add:

- start-here links
- core maps
- active work section
- review queue section

- [ ] **Step 3: Write `10 Wiki/LLM/LLM Index.md`**

Add:

- the purpose of the LLM knowledge area
- links to the LLM subfolders
- a short list of starter pages to create next

### Task 3: Add reusable note templates

**Files:**
- Create: `_templates/inbox-note.md`
- Create: `_templates/wiki-note.md`
- Create: `_templates/paper-note.md`
- Create: `_templates/project-note.md`
- Create: `_templates/daily-note.md`

- [ ] **Step 1: Write the inbox template**

Include source, raw capture, why-it-matters, and next-action sections.

- [ ] **Step 2: Write the wiki template**

Include one-line summary, why-it-matters, core idea, key details, links, and open questions.

- [ ] **Step 3: Write the paper template**

Include citation, summary, problem, contribution, understanding, and links back into wiki pages.

- [ ] **Step 4: Write the project template**

Include goal, current status, decisions, next actions, and related notes.

- [ ] **Step 5: Write the daily note template**

Include focus, notes, progress, questions, and links created today.

### Task 4: Seed the system with example notes

**Files:**
- Create: `00 Inbox/2026-07-09-welcome-capture.md`
- Create: `10 Wiki/LLM/Concepts/in-context-learning.md`
- Create: `40 Library/Papers/attention-is-all-you-need.md`
- Create: `20 Projects/second-brain-bootstrap/project.md`

- [ ] **Step 1: Write an inbox example**

Use a realistic quick-capture note that demonstrates how raw material enters the system.

- [ ] **Step 2: Write a wiki example**

Use `in-context-learning` as a concept page that shows durable-note style and related links.

- [ ] **Step 3: Write a paper example**

Use `Attention Is All You Need` as a paper note that points back to durable concept pages.

- [ ] **Step 4: Write a project example**

Create a bootstrap project note for evolving this second brain over time.

### Task 5: Verify usability

**Files:**
- Verify: all created files

- [ ] **Step 1: Review the created files for consistency**

Check naming, internal links, and whether the examples follow the templates.

- [ ] **Step 2: Review the directory tree**

Confirm the final structure matches the design and is easy to navigate.

- [ ] **Step 3: Do a start-here sanity check**

Read `README.md`, `10 Wiki/Home.md`, and `10 Wiki/LLM/LLM Index.md` in order and ensure a new user could begin without extra explanation.

## Self-Review

This plan covers the spec’s required scaffold, navigation, templates, sample notes, and minimum viable setup. It contains no unresolved placeholders and stays within the agreed scope of a local-first Markdown repository rather than adding automation or app-specific dependencies.
