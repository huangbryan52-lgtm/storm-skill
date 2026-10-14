# Stage 5 — Polish

The body is drafted and cited. Polish turns it into a finished, trustworthy
deliverable. Do these in order.

## 1. Write the lead section

Now that the body exists, write the lead (a 1–3 paragraph summary at the top,
under the title). It should:

- State what the topic is in the first sentence.
- Summarize the article's main points — every claim in the lead must already
  appear, sourced, in the body.
- Carry citations for any specific fact it states.

The lead is written last precisely so it reflects what the article actually
says.

## 2. Deduplicate and smooth

- Remove repeated facts that ended up in multiple sections (keep the best-placed
  instance).
- Add brief transitions between sections so the article reads as one piece.
- Check that heading levels are consistent and the order still flows.

## 3. Verify every citation

This is the integrity check — do not skip it.

- Every inline `[Sx]` in the text resolves to a row in `sources.md`.
- Every source in `sources.md` that you actually used appears in the final
  References list; drop unused rows from the References list (they can stay in
  `sources.md`).
- No `[CITATION NEEDED]` markers remain — resolve each by finding a source or
  cutting the claim.
- Spot-check 2–3 citations against their source snippets to confirm the claim
  matches what the source says. Fix any drift.
- No invented URLs, titles, dates, or authors.

## 4. Assemble the References list

Build the `## References` section from the used source IDs, in ID order:

```
## References
[S1] Author(s) (Year). *Title*. Publisher/Site. URL (accessed YYYY-MM-DD).
[S2] ...
```

Match the user's preferred citation format if they specified one.

## 5. Surface uncertainty to the user

In your message delivering the article (not buried in the article itself unless
asked), briefly note:

- Claims that were **contested** across sources and how you handled them.
- Areas with **thin sourcing** (single source, or weak source).
- Known **gaps** — questions from the research stage you couldn't source.

This honesty is part of the method; a confident article hiding weak sourcing is
worse than one that flags its limits.

## 6. Deliver

Save the final article to the working directory as `<topic-slug>.md` and
present it to the user, along with the short uncertainty note from step 5. Keep
the research artifacts (`sources.md`, etc.) available in case the user wants to
see the trail or extend the work.
