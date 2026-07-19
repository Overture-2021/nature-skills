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
- Position each claim against the prior belief it extends or overturns. Frame a
  contribution as a move from the established premise to the new one ("turning the
  static premise that X into a dynamic prediction of Y"), so the reader sees how the
  work builds on, and departs from, what the field already holds.

## 3. State the shape of the result up high; keep the numbers in Results

- In the abstract and introduction, state what was found — its direction and
  structure — not the full number ledger. Keep at most one or two headline anchors
  the reader should remember; move per-cell statistics, slopes, and intervals to
  Results and tables.
- The final introduction paragraph gives the contribution and the mechanism, not a
  recap of the measurements.
- Captions carry the message the figure makes, not the data behind it. Keep seed
  counts, per-cell statistics, confidence intervals, and step-by-step narration out
  of captions; let the figure do the work and put the numbers in the panel, a table,
  or an appendix. Say what the reader should conclude, once.

## 4. Advance the claim; cut defensive scaffolding

- Delete tail caveats and mid-sentence disclaimers from high-impact positions
  (abstract, introduction, contribution bullets, topic sentences): scope-hedges
  appended "just in case", `not X but Y` anti-misreading clarifications, and
  restatements of what the work does not claim. State each necessary boundary once,
  plainly, in Method, Discussion, or Limitations. This is the same instinct as the
  `anti-defensive-writing` pass; keep it on by default.
- Do not avoid overclaiming by negating. "X does not do Y", "X cannot Z",
  "detection holds regardless" read as defensive and often overclaim by implication.
  Reach the honest scope by choosing a more accurate *positive* claim about what the
  method does and where it holds — not by stacking up what it does not do.
- Keep a caveat only when it changes how the claim is read or used — validity,
  interpretation, scope, design, safety, or ethics. Do not scatter it into the
  summary.

## 5. Name things, and keep the names fixed

- Give the central method, system, router, or artifact a proper name and refer to
  it by that name everywhere, not by a rotating generic descriptor ("the routed
  policy", "our approach"). Introduce the name once, then reuse it (point 8 covers
  term-level consistency).

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

## 8. Keep terminology consistent across the whole paper

- Lock one canonical term for each recurring concept, method, model, dataset,
  metric, and symbol (see the Terminology Ledger), and use it uniformly across the
  entire paper — main text, appendix, tables, and figure captions alike. Do not let
  a second phrasing of a locked term reappear.
- When you rename or redefine a term, propagate the change everywhere in the same
  pass; leave no old variant behind. A term introduced in one section must read the
  same in every later reference to it.
- Sweep for two failure modes and fix them uniformly: the same object referred to
  two different ways, and one name or symbol reused for two different objects
  (de-conflate the second — give one a distinguishing subscript or a new name).
  Consistency across figures and captions matters as much as in the prose.

## 9. Write one idea per sentence

- Break a sentence that chains several claims with semicolons or em-dashes into
  separate sentences. A long multi-clause sentence that packs mechanism, evidence,
  and qualification together is the single most common thing the author rewrites by
  hand; if a sentence would earn a marginal note like "convoluted, simplify it", it
  is already too dense. Split it.
- A run of short declaratives beats one long periodic sentence. Prefer a period over
  a semicolon whenever the two halves can each stand alone.

## 10. Prefer natural phrasing over a repeated template

- Write what a person would actually write, not a slot-filled frame. When the same
  construction ("The <thing> is <property>.") recurs down a paragraph, vary the
  openings and the sentence shapes. The target is prose that no longer reads as
  generated from one template.

## 11. Keep the claims mutually consistent

- Adjacent and cross-section sentences must not contradict each other. When a
  revision changes what a sentence asserts — what was varied, what was held fixed,
  what a term denotes — re-read its neighbours and reconcile them in the same pass.
  A fluent paragraph that says "we switched the reward" in one line and "only
  difficulty changed" in the next is a defect even though each sentence reads well.
- Disambiguate an overloaded word instead of leaving the reader to guess, and define
  a term the first time it carries weight, not after it is already in use.

## 12. Revise with the lightest touch; make no uncommanded change

- This is the same discipline as `workflow.md` step 9, promoted to a standing house
  rule. Change only what was asked or flagged; keep the author's wording, ordering,
  and sentence structure verbatim everywhere else. Do not restore parallelism,
  re-polish a settled sentence, reflow a paragraph, or "improve" untouched text on
  your own initiative — an uncommanded edit gets reverted.
- When a change beyond the explicit ask seems warranted, propose it and wait; do not
  apply it silently. The author hand-writes the load-bearing sentences (title,
  abstract, definitions, key framing) and expects them preserved unless they say
  otherwise.

## Working from the author's inline `<...>` directives

The author edits by planting `<...>` notes directly in the source. Each is a task,
not a comment to read past. They recur in a few kinds:

- **Question** — "what about the other 2026 baselines?", "answer-matcher, is this
  word even given before?" Answer it in the prose (add the case, define the term) or
  surface that the material does not let you.
- **Missing content** — "Qwen3 is missing here, add it where appropriate",
  "fill in this blank". Supply it where it belongs.
- **Objection to the writing** — "this sentence is too convoluted, simplify it".
  Rewrite per points 9–12.
- **Consistency catch** — "reconcile this — I think the word 'test' is ambiguous".
  Fix the contradiction across the surrounding sentences (point 11).
- **Explicit tool call** — "use /anti-defensive-writing to rewrite this sentence".
  Apply that named pass to the marked span.

Resolve every marker, delete it from the draft, and report per marker what you did.
Never leave a marker in a delivered draft, and never silently drop one.
