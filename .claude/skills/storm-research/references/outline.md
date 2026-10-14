# Stage 3 — Outline

Build the article's structure *from the collected sources*, not from a generic
template or from memory. The outline is a plan for organizing what you actually
found.

## Procedure

1. **Cluster the sources.** Group the rows in `sources.md` by theme. The
   natural clusters usually map closely to the perspectives you used, but let
   the evidence regroup them — sometimes two perspectives collapse into one
   section, sometimes one splits into several.

2. **Draft the top-level sections** from the clusters. A typical long-form
   article has 4–8 top-level sections. Order them so the article reads
   logically (often: what it is → background → how it works → applications →
   limitations/criticism → future/comparison).

3. **Add subsections** where a section has enough distinct sourced material to
   warrant them. Don't create a subsection you can't fill with sources.

4. **Map sources to sections.** For each section and subsection, list the
   source IDs that support it. This is the critical check: **every section must
   map to at least one real source.** A section with no sources means either
   you're about to write from memory (stop — go collect sources) or the section
   shouldn't exist (cut it).

5. **Note the lead last.** Don't outline the lead/summary now; it's written
   after the body in the polish stage.

## Format (outline.md)

```
# <Title>

## 1. <Section>                          [S1][S3][S7]
   ### 1.1 <Subsection>                  [S3]
   ### 1.2 <Subsection>                  [S7][S9]
## 2. <Section>                          [S2][S5]
...
## References                            (auto-assembled from used IDs)
```

## Quality checks before writing

- Does the order flow for the confirmed audience?
- Is any single source carrying a whole section alone? If so, either find
  corroboration or scope the section down to what one source can support.
- Are contested points placed where you can present both sides?
- Is there a home for every major source? Orphan sources either reveal a
  missing section or were over-collected — decide deliberately.

Once every section maps to sources and the structure passes the outline gate in
`workflow.md`, move to writing.
