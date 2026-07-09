# LLM Core Pages Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add the first six core LLM concept pages and connect them into the existing LLM map.

**Architecture:** Create six concept notes under `10 Wiki/LLM/Concepts/` using the existing durable-note format, then update the LLM index to link to them as real pages rather than placeholders. Keep the pages concept-focused and cross-link them so the wiki starts behaving like a map rather than a folder of isolated notes.

**Tech Stack:** Markdown, local filesystem, Git

---

## File Structure

- Create: `10 Wiki/LLM/Concepts/transformer.md`
- Create: `10 Wiki/LLM/Concepts/attention.md`
- Create: `10 Wiki/LLM/Concepts/tokenization.md`
- Create: `10 Wiki/LLM/Concepts/pretraining.md`
- Create: `10 Wiki/LLM/Concepts/post-training.md`
- Create: `10 Wiki/LLM/Concepts/reasoning.md`
- Modify: `10 Wiki/LLM/LLM Index.md`

### Task 1: Write the six core concept pages

**Files:**
- Create: the six concept pages listed above

- [ ] **Step 1: Add `transformer.md`**

Explain the Transformer as the core sequence modeling architecture behind modern LLMs.

- [ ] **Step 2: Add `attention.md`**

Explain attention as the mechanism that lets tokens condition on one another.

- [ ] **Step 3: Add `tokenization.md`**

Explain tokenization as the representation layer between text and model computation.

- [ ] **Step 4: Add `pretraining.md`**

Explain pretraining as the large-scale base-model learning phase.

- [ ] **Step 5: Add `post-training.md`**

Explain post-training as the stage that makes base models more useful, aligned, and task-ready.

- [ ] **Step 6: Add `reasoning.md`**

Explain reasoning as the model behavior people care about, while noting the ambiguity of the term.

### Task 2: Connect the pages into the topic map

**Files:**
- Modify: `10 Wiki/LLM/LLM Index.md`

- [ ] **Step 1: Replace plain next-page names with real links**

Link the six new concept notes from the `Next Pages To Create` section.

- [ ] **Step 2: Keep the index readable**

Update only what is needed so the page remains compact and navigable.

### Task 3: Verify the knowledge map works

**Files:**
- Verify: the six concept files
- Verify: `10 Wiki/LLM/LLM Index.md`

- [ ] **Step 1: Read the concept pages for consistency**

Check that tone, structure, and depth match the existing `in-context-learning.md`.

- [ ] **Step 2: Check link coverage**

Confirm the pages reference each other meaningfully rather than living as isolated notes.

- [ ] **Step 3: Check index navigation**

Confirm the LLM index now points to real concept pages for the suggested next set.

## Self-Review

This plan is intentionally narrow: six concept pages plus minimal index linking. It matches the user request to “just start building the core pages” and avoids drifting into paper summaries, model cards, or system notes beyond what those concept pages need to explain themselves.
