# Stage 2 — Research (perspective-guided Q&A)

This is the heart of STORM. The quality of the final article is determined
here, not in the writing. Spend real effort. The goal is to populate
`sources.md` with broad, well-sourced coverage *before* any outline exists.

The stage has four steps: survey, discover perspectives, generate questions,
then search and collect.

## Step 1 — Quick survey

Run 1–3 broad searches to understand the topic's shape: what it is, its major
sub-areas, and the obvious landmarks. This is orientation, not collection yet —
though record any solid sources you hit into `sources.md`.

Use the survey to identify the topic's main facets. You'll turn those facets
into perspectives next.

## Step 2 — Discover perspectives

A single researcher asks a narrow band of questions. STORM's trick is to ask
from several **distinct expert viewpoints**, which widens coverage
dramatically.

Generate **3–6 perspectives** tailored to the topic. Each perspective is a
short persona + what it cares about. Draw them from the facets you found, plus
standard lenses:

- **Historical / origin** — how it came to be, timeline, precedents.
- **Technical / mechanistic** — how it works, architecture, methods.
- **Practical / applied** — use cases, adoption, who uses it and how.
- **Critical / skeptical** — limitations, failures, controversies, risks.
- **Comparative** — alternatives, competitors, how it differs from neighbors.
- **Economic / social / regulatory** — impact, cost, policy, ethics.
- **Future / trajectory** — where it's heading, open problems.

Pick the lenses that genuinely fit the topic (a biography needs different
lenses than a technology). Write them to `perspectives.md` with one line each
on what that viewpoint is after.

## Step 3 — Generate multi-perspective questions

For **each** perspective, write 4–8 concrete questions it would ask. Good
questions are specific and answerable by a source, not vague.

- Weak: "What about the history?"
- Strong: "When was the first working prototype demonstrated, and by whom?"

Group questions by perspective in `questions.md`. Across all perspectives you
should end up with roughly 20–40 questions. Deduplicate near-identical ones but
keep genuinely different angles even if they touch the same fact.

Optionally simulate a short back-and-forth per perspective: an answer to one
question often exposes the next, sharper question. Two or three follow-up
rounds per perspective is plenty.

## Step 4 — Search and collect

Now answer the questions by searching. For each question or cluster of related
questions:

1. Run a targeted search. Batch independent searches in one turn.
2. For promising results, fetch the page to read it properly rather than
   trusting the snippet.
3. Extract the specific claim that answers the question and add a row to
   `sources.md` with a real title, URL, and access date.
4. If results conflict, record **both** sources and note the conflict — you'll
   surface it in the article.

Prioritize:
- **Primary and authoritative sources** (papers, official docs, standards,
  original announcements) over aggregators and SEO content.
- **Recency** where the topic moves fast; **durability** where it doesn't.
- **Diversity** of sources — avoid citing five pages that all copy one origin.

Stop when coverage is sufficient: every perspective has real sources, and no
major planned sub-topic sits at zero sources. It's fine to leave a known gap —
note it rather than inventing filler.

## Anti-patterns

- Writing questions and then answering them from memory. **Search.**
- Collecting ten sources that all restate the same press release.
- Skipping the critical/skeptical perspective because the topic seems settled.
- Adding a source row you didn't actually open and verify.

When `sources.md` passes the research gate in `workflow.md`, move to the
outline stage.
