---
name: storm-research
description: >-
  Research and write a long-form, well-cited article on a topic from scratch
  using the STORM method (Synthesis of Topic Outlines through Retrieval and
  Multi-perspective Question asking). Use when the user asks for a thorough
  research report, a Wikipedia-style article, a background briefing, a
  literature-style survey, or a deeply-sourced write-up on an unfamiliar topic
  and wants it grounded in citations rather than recalled from memory.
---

# STORM Research

STORM turns a bare topic into a grounded, citation-backed article by **doing
the research before writing**. Instead of drafting from memory, you discover
what questions matter, search for answers, build an outline from the collected
sources, then write each section strictly from those sources.

The method comes from Stanford's STORM paper (Shao et al., 2024). The core
insight: good research questions come from *multiple perspectives*, not one.
Simulate several expert viewpoints interrogating the topic, and the coverage
gets far broader than a single researcher's default questions.

## When to use this

Use STORM when the user wants depth and trustworthy sourcing:

- "Write me a report on …" / "Research … and write it up"
- "Give me a Wikipedia-style article on …"
- "I need a thorough briefing on …" for an unfamiliar area
- Any long-form write-up where claims must be traceable to sources

Do **not** use STORM for quick factual answers, opinion pieces, creative
writing, or tasks where the user already supplied all the source material and
just wants it summarized (summarize it directly instead).

## The pipeline

Work through five stages in order. Each stage has a dedicated reference file —
read it when you reach that stage, not before.

1. **Scope** — pin down the topic, audience, depth, and length with the user.
2. **Research (perspective-guided Q&A)** — discover perspectives, generate
   multi-perspective questions, search, and collect cited snippets into a
   source table. See `references/research.md`.
3. **Outline** — synthesize the collected sources into a hierarchical outline.
   See `references/outline.md`.
4. **Write** — draft each section grounded *only* in collected sources, with
   inline citations. See `references/writing.md`.
5. **Polish** — add a lead/summary, dedupe, verify every citation, assemble the
   reference list. See `references/polish.md`.

Checklists and the output file layout live in `references/workflow.md`. Read it
once at the start of a run.

## Core rules (do not skip)

- **Research before writing.** Never draft a section until its sources are
  collected. If you catch yourself writing from memory, stop and search.
- **Every non-obvious claim gets a citation** mapped to a real collected
  source. No citation without a source; no invented sources or URLs.
- **Perspectives drive coverage.** Generate questions from 3–6 distinct
  viewpoints, not one. This is what separates STORM from a generic outline.
- **Keep a source table** throughout so citations in the draft trace back to
  actual search results.
- **Surface uncertainty.** Flag contested claims, thin sourcing, and gaps
  rather than papering over them.

## Fast start

1. Read `references/workflow.md` for the output layout and checklists.
2. Confirm scope with the user (one short round of questions).
3. Run the research stage (`references/research.md`) — this is the heart of
   STORM; spend real effort here.
4. Outline, write, polish using the remaining reference files.
5. Deliver the article plus its reference list as a markdown file.
