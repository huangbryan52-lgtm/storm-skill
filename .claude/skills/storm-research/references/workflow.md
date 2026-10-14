# Workflow, output layout, and checklists

Read this once at the start of a STORM run. It covers how to set up working
files, what the final deliverable looks like, and the gate checklist for each
stage.

## Working files

Keep research artifacts separate from the final article so the draft stays
clean and citations stay traceable.

Use the scratchpad for intermediate state and the working directory (or a
user-specified location) for the deliverable:

```
<scratchpad>/storm/
  perspectives.md     # the viewpoints you generated
  questions.md        # multi-perspective questions, grouped by perspective
  sources.md          # the source table (see below) — the citation ledger
  outline.md          # the working outline
<working dir>/
  <topic-slug>.md     # the final article (the deliverable)
```

If the scratchpad path is unknown, put the `storm/` folder under the working
directory instead and mention it to the user.

## The source table (sources.md)

This is the backbone of STORM. Every citation in the final article must map to
a row here. Maintain it as you search:

```
| ID  | Claim / snippet (short)                     | Source title           | URL                        | Date accessed |
|-----|---------------------------------------------|------------------------|----------------------------|---------------|
| S1  | STORM uses multi-perspective question gen   | Shao et al. 2024       | https://arxiv.org/abs/...  | 2026-10-14    |
| S2  | ...                                         | ...                    | ...                        | ...           |
```

Rules:
- One row per distinct source-backed fact or claim. Reuse an ID for repeated
  use of the same fact.
- Never add a row you did not actually retrieve from a search result or a
  user-supplied document. No placeholder or guessed URLs.
- Keep the snippet short but specific enough to verify the claim later.

## Final article layout

```markdown
# <Title>

<Lead section: 1–3 paragraph summary of the whole article, written last.>

## <Section 1>
Prose with inline citations [S1][S4] ...

### <Subsection 1.1>
...

## <Section 2>
...

## References
[S1] Shao et al. (2024). *Assisting in Writing Wikipedia-like Articles...* https://arxiv.org/abs/...
[S2] ...
```

Citation style: inline bracketed source IDs `[S1]` that resolve against the
References list. If the user prefers footnotes, numbered `[1]` style, or a
specific academic format, follow their preference instead — ask if unsure.

## Stage gate checklist

Do not advance to the next stage until the current one passes its gate.

**Scope gate**
- [ ] Topic, audience, target depth/length, and citation style confirmed.

**Research gate**
- [ ] 3–6 distinct perspectives written to `perspectives.md`.
- [ ] Multi-perspective questions written to `questions.md`.
- [ ] Searches run; `sources.md` populated with real, retrieved sources.
- [ ] Coverage feels sufficient for the confirmed scope (no major sub-topic
      with zero sources).

**Outline gate**
- [ ] Hierarchical outline built *from* the sources, not from memory.
- [ ] Every planned section maps to at least one source ID.

**Writing gate**
- [ ] Each section drafted only from collected sources.
- [ ] Every non-obvious claim carries a citation to a real source ID.

**Polish gate**
- [ ] Lead section written and accurate to the body.
- [ ] Duplication removed; sections flow.
- [ ] Every `[Sx]` in the text exists in References; every reference is used.
- [ ] Contested/thin claims flagged; gaps noted to the user.

## Tooling notes

- Prefer the environment's search tool (e.g. `WebSearch`) for discovery and
  `WebFetch` to read a specific page in depth. Batch independent searches.
- If the user supplied documents, treat them as first-class sources (give them
  source IDs too) and read them before searching the open web.
- Respect the repository/network scope and the user's data-sharing
  expectations when searching externally.
