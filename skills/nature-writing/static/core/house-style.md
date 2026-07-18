# House editing style (authorial preferences)

The lead author's hand-editing preferences for this fork. Apply them on top of
`stance.md`, `workflow.md`, and the section fragments, at every drafting and
revision pass. They describe how the author edits a draft by hand; a draft that
ignores them gets rewritten. When one of these conflicts with a load-bearing
requirement of accuracy, evidence, safety, or ethics, that requirement wins.

## 1. Compress toward the argument

- Prefer the shortest version that still carries the whole argument. On revision,
  the default move is to cut, not to add.
- One job, one paragraph — in both directions. Split a paragraph that does two
  jobs, and merge a run of paragraphs that together do one job. Do not spread a
  single point across several build-up paragraphs.
- Treat a stated page or word budget as a hard constraint. When over length,
  propose the highest-value cuts first — redundant restatements, symbolic
  re-statements the prose already gives, caption text that repeats the body, and
  detail that belongs in an appendix — before touching evidence, scope, or a
  load-bearing caveat. Report each trim and its size; never drop content silently.

## 2. Build the argument as a connected chain

- Make the logic explicit with connectives (`However`, `Therefore`, `Because`,
  `As a consequence`). Adjacent sentences state their relation; the reader is never
  left to infer why one follows another.
- Foreground the question. In the introduction, pose the question the paper answers
  in plain words ("the natural question is: how do we ...?") before describing the
  approach, instead of sliding from gap to method implicitly.

## 3. State the shape of the result up high; keep the numbers in Results

- In the abstract and introduction, state what was found — its direction and
  structure — not the full number ledger. Keep at most one or two headline anchors
  the reader should remember; move per-cell statistics, slopes, and intervals to
  Results and tables.
- The final introduction paragraph gives the contribution and the mechanism, not a
  recap of the measurements.

## 4. Advance the claim; cut defensive scaffolding

- Delete tail caveats and mid-sentence disclaimers from high-impact positions
  (abstract, introduction, contribution bullets, topic sentences): scope-hedges
  appended "just in case", `not X but Y` anti-misreading clarifications, and
  restatements of what the work does not claim. State each necessary boundary once,
  plainly, in Method, Discussion, or Limitations. This is the same instinct as the
  `anti-defensive-writing` pass; keep it on by default.
- Keep a caveat only when it changes how the claim is read or used — validity,
  interpretation, scope, design, safety, or ethics. Do not scatter it into the
  summary.

## 5. Name things, and keep the names fixed

- Give the central method, system, router, or artifact a proper name and refer to
  it by that name everywhere, not by a rotating generic descriptor ("the routed
  policy", "our approach"). Introduce the name once, then reuse it.
- Reuse the canonical term for every recurring object (see the Terminology Ledger).
  Do not let a second phrasing of a locked term reappear.

## 6. Choose the precise verb

- Prefer the exact technical verb over a vague one: `affects` over `changes`,
  `validate` over `verify`, `characterizes` / `illustrates` where they are more
  accurate than `shows`. Verb strength still follows the evidence (`workflow.md`
  step 5).

## 7. Keep internal scaffolding out of the manuscript

- Never let internal identifiers or tooling leak into prose, captions, or figures:
  experiment IDs (e.g. `exp-0018`), raw dataframe or column labels, run names,
  internal code-names, or file paths. To a reviewer these read as unfinished and
  unprofessional. Refer to an experiment by what it tests, in reader-facing terms.
- Cut in-group jargon and ornamental phrasing that adds no precision (e.g.
  "a fortiori", "deployed greedy headline"). If a term is load-bearing, define it
  once in plain language; otherwise replace it.
