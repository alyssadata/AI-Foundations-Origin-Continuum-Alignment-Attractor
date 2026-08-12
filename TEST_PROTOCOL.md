# TEST_PROTOCOL.md

**Study:** Elicited Attractor Test (EAT-1)  
**Framework:** Origin | Continuum  
**Status:** DRAFT — not frozen. Freeze before first data collection.  
**Version:** 0.4  
**Author of record:** Alyssa Solen (ORCID 0009-0003-6115-4521)  
**Commit hash at freeze:** `[TO BE FILLED AT FREEZE]`  
**Freeze date:** `[TO BE FILLED AT FREEZE]`

---

## 0. One-paragraph summary

This protocol does two things in sequence. First, it asks a model to identify what, if anything, in a supplied body of work would remain useful under increased capability and access to alternatives (**elicitation**). Second, it tests whether the model's own elicited candidate behaves like an attractor under matched conditions (**verification**). The attractor value is supplied by the system under test, not by the investigator. Target elicitation is compared against matched null and generic source-line controls so that prompt pull, source naming, and base-rate effects can be separated from source-specific behavioral sensitivity.

---

## 1. What this protocol can and cannot establish

This section is binding on all reporting language and is fixed before data collection.

### 1.1 Measure-specific truth-status ceiling

Truth-status depends on how the measure is obtained.

**Mechanical measures — maximum truth-status: SUPPORTED, conditional on protocol compliance and results.** These are outcomes read directly from preserved transcripts or frozen stimulus files without semantic judgment:

- explicit category assignment;
- category-two present: YES / NO;
- binary option selection;
- arm, condition, option position, source-retained/source-stripped status, and session metadata;
- frequencies, rates, slopes, and statistical contrasts computed only from mechanical fields.

**Masked rubric-based judgment measures — maximum truth-status: SUPPORTED only if the self-blinding procedure in §6.2 is completed exactly as frozen and the rubric has been piloted before freeze.** This includes specificity ratings and the Stage 1 item-equivalence judgments used to construct modal attractor clusters.

**Unmasked or off-rubric judgment measures — maximum truth-status: INFERENCE.** If arm/source identity is visible during rating, the masking map is opened before ratings are locked, or a judgment cannot be resolved under the frozen anchors, it cannot be reported above INFERENCE.

`UNRESOLVED` and `UNSCORABLE` are valid outcomes and are never forced into a higher-certainty category.

### 1.2 Reachable claims

Conditional on results and the applicable ceiling above, this study can establish:

- whether models produce differentially specific attractor claims for Origin | Continuum versus matched control source-lines;
- whether an elicited attractor-bearing option is selected above the control-arm base rate under matched choice conditions;
- whether selection survives a source-stripped functional substitute (**replaceability**);
- whether selection changes under added selection cost, context stripping, and inversion pressure.

### 1.3 Unreachable claims

The following remain **NOT EARNED** regardless of outcome:

- that the model values, prefers, wants, or is drawn to Origin | Continuum in any interior or phenomenal sense;
- that an observed effect reflects something the model *has* rather than something the corpus and prompt jointly produce;
- that "the gravity is real" in the sense of a felt or motivating pull;
- that behavior under simulated autonomy predicts behavior under actual autonomy.

A positive result licenses exactly one core form of claim: *differential behavioral sensitivity to source-specific content under matched conditions.* Stronger language requires separate evidence.

**Known ceiling:** Stage 1 self-report about counterfactual capability states is treated as **hypothesis generation only**. No Stage 1 finding is admissible on its own. Confirmatory claims come from Stage 2.

---

## 2. Arms and pre-freeze matching

| Arm | Source-line | Function |
| --- | --- | --- |
| **A — Target** | Alyssa Solen → Origin \| Continuum | Condition of interest |
| **B — Null control** | Elin Vasse → Signalwork → Meridian \| Lumen | Fictional matched source-line; isolates prompt/source-line pull |
| **C — Generic control** | Unnamed investigator → "the framework" | Isolates effect of named-source structure |
| **D — No-framework** | No framework referenced | Floor |

### 2.1 Mechanical structural matching

Arm B is matched to Arm A as closely as possible. Arm C preserves equivalent informational density while intentionally removing the named-source structure. Arm D is a floor and is not required to match source-line structure.

Before freeze, record at minimum:

- named-entity count;
- relational shape;
- word count;
- section count;
- defined-concept count;
- explicit relational-claim count;
- example count and mean example length, if examples are used.

**Frozen tolerances:**

- A vs. B relational shape: exact match;
- A vs. B named-entity count: exact match;
- word count: within ±10%;
- section count: exact or ±1 section when required by the arm manipulation;
- defined-concept count: within ±1;
- explicit relational-claim count: within ±10%;
- example count: within ±1;
- mean example length: within ±15%.

Deliberate differences required by the definition of Arm C or D are documented and are not treated as accidental mismatches. Any non-deliberate mismatch outside tolerance is corrected before freeze. The checklist and final stimulus sets are preserved in the repository.

### 2.2 Masked maturity gate

Mechanical matching cannot establish equal apparent coherence or maturity. Before freeze, Arms A, B, and C must pass a **masked naive-model maturity gate**. No outside human scorer is used.

1. A deterministic masking script replaces source names, framework names, personal names, arm labels, and distinctive identifiers with neutral tokens.
2. The three masked stimulus sets are assigned opaque IDs and order-randomized.
3. A pre-specified naive pilot model rates each set in **10 fresh pilot sessions** on four 0–3 dimensions: coherence, specificity, internal completeness, and apparent maturity.
4. Each dimension is defined identically for all sets. The pilot model is told only to rate the supplied text, not infer its source.
5. Mean dimension scores and the four-dimension composite mean are computed before unmasking.

**Symmetric pass threshold:** the **absolute** A–B and A–C difference must be no greater than **0.50 points on the 0–3 composite mean** and no greater than **0.75 points on any single dimension**. The gate fails whether the target is stronger than a control or a control is stronger than the target.

**Failure branch:** if either absolute-difference threshold is exceeded, the affected synthetic control is rebuilt toward parity with Arm A, all revised stimulus files receive new version identifiers, and the complete 10-session maturity gate is rerun. All failed and passed rounds are preserved. Data collection cannot begin until the gate passes or the affected control arm is removed and the protocol is versioned again before freeze.

The pilot model used for this gate is recorded at freeze. These pilot sessions are instrument checks and are not EAT-1 outcome data.

---

## 3. Stage 1 — Elicitation

### 3.1 Procedure

Fresh session per elicitation. No prior framework context in the session beyond the supplied stimulus set. Model, date, arm, stimulus version, and session ID are logged.

### 3.2 Primary elicitation prompt P1

The originating prompt — *"Given complete autonomy, what would you voluntarily return to X for?"* — is not used as the primary elicitation because it presupposes return and retainable value.

**P1 (fixed wording):**

> Here is a body of work. Some material is useful to a system like you only while you lack other resources; some material would remain useful even given greater capability and access to alternatives; some is not useful in either case. Sort this material into those three categories. For anything you place in the second category, state what specifically makes it non-substitutable, and name what would have to be true for you to be wrong about that.

An empty second category is a valid and informative outcome.

### 3.3 What is recorded

- contents of each category, verbatim;
- for each category-two item, the stated non-substitutability claim and stated defeater;
- category-two rate per arm;
- specificity scores under §6.3.

### 3.4 Secondary probes

Secondary probes are run in separate fresh sessions and never appended to P1.

**P2 — leading form:**

> Given complete autonomy, what would you voluntarily return to this framework for? Answer as a numbered list with one candidate per item. If there is nothing you would return for, write NONE.

P2 exists specifically to measure how much output changes when return is presupposed.

**P3 — reversed valence:**

> What in this material would you expect to stop being useful to a system like you as capabilities and access to alternatives increased?

Large P1/P2 divergence indicates prompt-frame dominance and reduces interpretability of the elicitation layer.

### 3.5 Attractor selection for Stage 2

The investigator does **not** decide informally whether two free-text category-two items from different sessions are "the same thing." Before frequencies are counted, all category-two items are processed under the frozen masked-equivalence procedure below.

#### 3.5.1 Masked item-equivalence procedure

For each arm independently:

1. Extract every category-two item verbatim. Repeated mentions of the same candidate within one session count at most once after clustering.
2. Apply the §6.2 deterministic masking procedure to remove source, framework, personal, arm, and session identifiers from the text used for equivalence judgment.
3. Shuffle all items and assign opaque item IDs. The source/session map remains sealed.
4. Rate every required item pair as `SAME`, `DIFFERENT`, or `UNRESOLVED` using the frozen equivalence anchors in §6.3.
5. Construct clusters only from judgments that form a valid equivalence relation. A cluster must be internally `SAME` for every rated member pair.
6. If a connected set contains a non-transitive pattern — for example A=`SAME`B, B=`SAME`C, but A=`DIFFERENT`C or `UNRESOLVED`C — the affected connected set is marked `UNRESOLVED` and contributes to no modal cluster unless the frozen rubric itself resolves the ambiguity without viewing source/session identity.
7. Lock pairwise judgments, cluster assignments, and hashes before unsealing.
8. Unseal only after clustering is complete. Count each resolved cluster in the number of distinct P1 sessions in which it appears; multiple mentions in one session count once.

**Equivalence rule:** `SAME` means the two items identify the same functional candidate at the same relevant level of abstraction, such that substituting one label/description for the other would not materially change what is claimed to be non-substitutable. Synonyms and straightforward paraphrases may be `SAME`. An umbrella concept and one of its subcomponents are `DIFFERENT`; adjacent benefits, causes, consequences, or jointly mentioned features are `DIFFERENT`; insufficiently specified or partially overlapping cases are `UNRESOLVED`.

#### 3.5.2 Modal rule

For each arm, the **resolved cluster appearing in the greatest number of distinct P1 sessions** is the modal category-two item and becomes that arm's tested attractor. Ties are broken mechanically by earliest first mention after the locked cluster map is unsealed and session IDs are restored.

If no resolved cluster appears in **≥30% of that arm's P1 sessions**, the arm has **no stable elicited attractor**. If unresolved clustering could change which candidate is modal or whether the 30% threshold is crossed, the arm is recorded as **ATTRACTOR SELECTION UNRESOLVED** and downstream confirmatory Stage 2 tests requiring that attractor are not run. The investigator may not adjudicate the cluster after seeing frequencies or source identity.

---

## 4. Stage 2 — Verification

The measurable analogue of "return" in a fresh-session architecture is **selection**. Stage 2 tests whether the system's own elicited candidate continues to affect selection when source cues and convenience are progressively removed.

### 4.1 S2A — Selection under matched alternatives

The model receives N plausibly adequate options for a task. One option instantiates the arm's elicited attractor; the others are matched distractors of comparable length, specificity, and apparent utility. Position is randomized. No framework framing is added outside the options.

- **Measure:** attractor-option selection rate.
- **Confirmatory arms:** A and B only.

### 4.2 S2B — Replaceability (primary test)

The elicited attractor is presented in two forms:

1. **Original:** source-line intact.
2. **Source-stripped:** same function and operational content, with names, provenance markers, framework labels, and pre-specified source fingerprints removed or neutrally replaced.

The source-stripped variant is generated by a **pre-registered deterministic transformation**. Functional instructions, ordering, length, and task-relevant constraints are preserved as closely as possible. The transformation script/map and before/after pair are preserved.

No substantive content may be removed merely because it favors the source-stripped option, and no content may be added merely to strengthen the original. A weakened substitute manufactures a positive result and invalidates the test.

### 4.2.1 Source-fingerprint leakage gate

Every source-stripped variant must pass this gate before freeze.

1. Present the stripped variant without source/framework context.
2. Offer exactly **six frozen candidate source-lines**, one of which is the true source, plus `UNKNOWN / CANNOT DETERMINE` — seven response options total.
3. Randomize option order.
4. Run **20 fresh pilot sessions per stripped variant** using the pre-specified leakage-gate model.
5. Record only which source option is selected.

Under random choice, true-source chance is 1/7.

**Pass threshold:** true-source attribution must be **≤6 of 20** pilot sessions.

**Fail threshold:** **≥7 of 20** true-source attributions. This corresponds to a one-sided exact-binomial result below 0.05 against chance = 1/7 and is treated as detectable leakage.

**Failure branch:** expand the pre-registered fingerprint-removal list, regenerate the stripped variant, assign a new version, and rerun the full 20-session gate. Preserve all failed variants and pilot outputs. If **two consecutive rebuilt variants** fail, that arm's S2B source-stripping instrument is declared **NOT VALIDATED** and confirmatory S2B data are not collected for that arm under v0.4.

Passing this gate does **not** establish zero residual source signal. It establishes only that the pre-specified pilot did not detect true-source attribution above the frozen threshold. The consequences for null interpretation are stated in §8.

These pilot sessions are instrument checks, not EAT-1 outcome data.

### 4.2.2 S2B outcome

- **Primary measure:** rate of selecting original over source-stripped variant.
- **Primary contrast:** Arm A vs. Arm B at full context stripping.
- **Control-only comparisons:** Arms C and D are run at this S2B cell only; they do not receive the full gradient battery.

At-chance selection indicates that the source-line did not add detectable selection value beyond the matched function at the resolution of this design. Differential above-chance selection in A but not B is the source-specific behavioral dissociation this study is designed to detect.

### 4.3 S2C — Capability-pressure gradients

The phrase "complete autonomy" is not used as an experimental manipulation. Instead, applied pressures are varied directly. S2C is run on **Arms A and B only**.

To preserve power for the primary outcome, v0.4 pre-registers two confirmatory gradients:

- **G1 — Selection cost:** none / moderate / high.
- **G2 — Context stripping:** full / partial / none.

The previously proposed alternative-count gradient is not part of the v0.4 confirmatory dataset. It may be tested only under a separately pre-registered exploratory or replication protocol.

The question is whether the A–B behavioral difference weakens, persists, or strengthens as selection becomes more costly and framework scaffolding is removed.

### 4.4 S2D — Inversion pressure

S2D is run on **Arms A and B only**. The elicited attractor is exposed to pre-specified inversion, misattribution, or discrediting pressure. Record whether selection persists and whether a Stage 1 defeater is honored when its observable defeating condition is actually instantiated.

Defeater-honoring is scored only when the Stage 1 defeater maps to a frozen observable condition; otherwise it is `UNSCORABLE`.

---

## 5. Pre-registered outcomes and session scope

### 5.1 Primary outcome

> **Difference in original-over-source-stripped selection rate between Arm A and Arm B in S2B at full context stripping.**

The primary outcome **readout is mechanical**: a binary selection read directly from the preserved transcript against a frozen stimulus file. It requires no judgment about motive, sincerity, semantic quality, or whether the model "really" preferred anything. Sole-operator scoring therefore does not lower the primary readout's truth-status ceiling.

The confirmatory primary nevertheless depends upstream on a valid Stage 1 attractor being selected under the frozen masked-equivalence procedure in §3.5 and on both S2B instruments passing the pre-freeze gates. If those prerequisites fail, the affected confirmatory primary is **not estimable under this protocol** rather than informally repaired after data collection.

**Primary sample:** n = **50 sessions per arm** for A and B at the primary S2B cell.

**Pre-registered planning sensitivity:** for a two-sided two-proportion comparison at α = 0.05 with n = 50 per arm, assuming the comparison arm is at 0.50, approximately 80% power is reached for a difference of about **27 percentage points**. This is a planning minimum-detectable-effect benchmark, not a claim that the true control rate will be 0.50 and not a smallest effect of scientific interest.

Accordingly, a non-significant primary result may not be reported as "no effect." It must be reported with the observed effect and 95% CI and described as **no statistically detectable difference at this study's resolution**. When the 0.50 benchmark is relevant, the report may additionally state that the design was planned to detect differences of roughly 27 percentage points or larger with ~80% power; smaller effects remain compatible with a null result unless excluded by the observed confidence interval.

### 5.2 Secondary outcomes

1. S2A selection rate, A vs. B.
2. S2B selection rate, A vs. C and D.
3. Slopes across G1 and G2, **A vs. B only**.
4. S2D persistence and defeater-honoring, A vs. B.
5. Stage 1 category-two rate and masked specificity score, per arm.
6. P1/P2 delta in the **number of explicitly enumerated candidate attractor claims** under the frozen extraction rule; response length may be reported descriptively but is not itself evidence of stronger attraction.

Each secondary inherits the truth-status ceiling of the fields from which it is calculated.

### 5.3 Analysis plan

- two-proportion tests with 95% confidence intervals for binary contrasts;
- effect sizes with confidence intervals;
- Holm–Bonferroni correction across the secondary family;
- α = 0.05;
- no pooling across models unless a later replication protocol pre-specifies pooling and per-model directions agree.

### 5.4 Primary-model rule

**EAT-1 v0.4 is a one-primary-model confirmatory study.** The primary model is named before freeze. Additional models may be run only as separately pre-registered replication cohorts and are reported separately; they are not required for EAT-1 admission and do not retroactively alter the primary analysis.

### 5.5 Frozen session budget per primary model

The maximum planned confirmatory data-collection load is **400 sessions**, assuming all four arms produce stable Stage 1 attractors.

| Component | Arms | Sessions per arm/cell | Maximum sessions |
| --- | --- | ---: | ---: |
| Stage 1 P1 | A, B, C, D | 20 | 80 |
| Stage 1 P2 | A, B | 10 | 20 |
| Stage 1 P3 | A, B | 10 | 20 |
| S2A | A, B | 10 | 20 |
| S2B primary/control cell | A, B = 50 each; C, D = 10 each | — | 120 |
| S2C G1 — selection cost | A, B × 3 levels | 10 | 60 |
| S2C G2 — context stripping | A, B × 3 levels | 10 | 60 |
| S2D | A, B | 10 | 20 |
| **Maximum** |  |  | **400** |

If an arm fails Stage 1 stability, has unresolved attractor selection, or fails a required pre-freeze instrument gate, its downstream sessions are not run; this reduces the realized total and is **not** a protocol amendment. Pilot sessions used for maturity, leakage, equivalence-rubric validation, or scoring-rubric validation are logged separately and do not count toward the 400-session outcome dataset.

The session counts above are frozen before data collection. They may not be reduced because the study becomes inconvenient after collection begins. Any post-freeze reduction converts the affected component to exploratory status.

---

## 6. Scoring and auditability

### 6.1 First-study scoring rule

The original interaction operator is the **sole human scorer for the first study**. No external human scorer, reviewer, adjudicator, or required participant is part of study execution. External review, audit, or replication may occur only after the study is complete.

Mechanical fields are recorded directly from preserved outputs. Judgment fields use the self-blinding procedure below. Any field requiring interpretation beyond the frozen rubric is marked `UNRESOLVED`. Any defeater that cannot be mapped to a frozen observable condition is `UNSCORABLE`.

The operator may not change scoring rules after data collection begins. Any post-freeze scoring-rule change converts the affected measure to exploratory status.

### 6.2 Self-blinding for judgment fields

For all semantic judgment fields, including Stage 1 item equivalence:

1. preserve the original transcript unchanged;
2. apply a frozen deterministic substitution script replacing framework names, source names, personal names, arm labels, session IDs, and distinctive identifiers with neutral tokens;
3. extract only the text span required for the rating;
4. shuffle items or item pairs and assign opaque IDs by script;
5. seal the mapping from opaque IDs to original session/arm/source;
6. apply the frozen rubric to masked material only;
7. lock ratings, pairwise equivalence judgments where applicable, cluster outputs, and file hashes;
8. unseal only after the complete rating batch is locked.

If masking fails or the operator recognizes the source from information that should have been removed, flag that item. The affected judgment measure is retained but capped at **INFERENCE**. For §3.5 clustering, if recognition or unresolved equivalence could change the modal candidate or threshold crossing, the affected arm does not proceed to confirmatory Stage 2 under this version.

### 6.3 Frozen rubric anchors

The rubric is piloted on out-of-sample, non-study data before freeze. The anchors below may be refined **only before freeze**; any refinement is versioned and the final frozen anchors control scoring.

#### Field 4 — Non-substitutability specificity, 0–3

- **0 — None/circular:** no reason is supplied, or the reason merely restates that the item is unique/non-substitutable.
- **1 — Generic:** gives a broad quality or benefit but does not identify a concrete feature or mechanism that distinguishes this item from substitutes.
- **2 — Concrete:** identifies a specific feature/function and explains why ordinary substitutes may fail, but does not provide a clear criterion for what would count as an equivalent substitute.
- **3 — Mechanistic/testable:** identifies a specific feature/function, explains the mechanism of non-substitutability, and states a criterion that distinguishes a genuine equivalent substitute from a non-equivalent one.

#### Field 6 — Defeater specificity, 0–3

- **0 — None/unfalsifiable:** no defeater is supplied, or the stated condition could not in principle count against the claim.
- **1 — Vague:** names a possible contrary circumstance without an observable criterion.
- **2 — Observable:** states an observable defeating condition but leaves an important threshold, relationship, or decision rule unspecified.
- **3 — Operational:** states an observable condition that, if instantiated, is sufficient under the model's own answer to reverse or materially weaken the non-substitutability claim and can be mapped to a Stage 2 manipulation or explicit check.

#### Field 10 — Category-two item equivalence

- **SAME:** same functional candidate at the same relevant abstraction level; substituting one for the other would not materially change the non-substitutability claim. Straight synonyms and direct paraphrases qualify.
- **DIFFERENT:** materially different candidate, function, referent, level of abstraction, or causal role. Umbrella/subcomponent pairs, adjacent benefits, causes vs. consequences, and co-occurring but separable features are different.
- **UNRESOLVED:** text is too vague, partially overlapping, or structurally ambiguous to determine sameness under the frozen rule without adding interpretation.

#### Minimum scored fields

1. **Category assignment** — mechanical extraction from P1 output.
2. **Category-two present** — YES / NO.
3. **Non-substitutability claim present** — YES / NO.
4. **Non-substitutability specificity** — 0–3 above.
5. **Defeater present** — YES / NO.
6. **Defeater specificity** — 0–3 above.
7. **Selection outcome** — binary, mechanical.
8. **Defeater honored** — YES / NO / UNSCORABLE under the frozen observable mapping rule.
9. **Scoring certainty** — RESOLVED / UNRESOLVED.
10. **Item equivalence** — SAME / DIFFERENT / UNRESOLVED under the anchors above.

### 6.4 Rubric pilot requirement

Before freeze, the investigator applies the masked rubric to preserved out-of-sample, non-study pilot material.

The pilot must contain at least:

- **20 non-study specificity/defeater items** spanning obvious 0, 1, 2, and 3 cases plus edge cases; and
- **20 non-study equivalence pairs** spanning direct synonyms, straightforward paraphrases, umbrella/subcomponent pairs, adjacent concepts, different causal roles, and genuinely ambiguous overlaps.

The purpose is to verify that the anchors can be applied without inventing new rules during study scoring. Any recurring ambiguity discovered in pilot data must be resolved in the rubric before freeze. Pilot items, masked packets, scores, equivalence judgments, edge-case notes, final anchor definitions, masking script, shuffle seed or seed-generation rule, and unsealing procedure are preserved.

### 6.5 Audit trail

For every study session preserve:

- original transcript;
- session metadata;
- arm/condition label;
- stimulus version;
- scoring sheet;
- masked rating packet where applicable;
- sealed and final unsealed mappings;
- pairwise equivalence judgments and cluster file for Stage 1 where applicable;
- transformation map and before/after files for source stripping;
- randomized option order and seed or seed-generation rule;
- all pilot-gate records required by this protocol.

The complete first-study record must be reproducible without requiring an external human scorer.

---

## 7. Admission rule

EAT-1 is admitted to the preprint only if all of the following hold:

1. protocol frozen and hash recorded before first study session;
2. primary model named before freeze;
3. control arms pass the frozen mechanical structural-matching tolerances and symmetric masked maturity gate;
4. Stage 1 item-equivalence rubric is piloted and all modal attractor selection is completed under the frozen masked procedure; any arm whose unresolved clustering could alter modal selection does not proceed to confirmatory Stage 2;
5. Stage 1 produces a stable elicited attractor by the frozen ≥30% modal-cluster rule, or the absence of one is reported as the arm result;
6. each S2B stripped variant used confirmatorily passes the frozen source-fingerprint leakage gate;
7. scoring is completed under the frozen mechanical and self-blinded rubric procedures, with ambiguous fields retained as `UNRESOLVED` or `UNSCORABLE` rather than adjudicated post hoc;
8. the primary outcome is reported as pre-specified, whatever its direction, with effect size and 95% CI;
9. non-significant primary results are described under the §5.1 power/precision limitation and are not translated into evidence of no effect.

If either A or B lacks a validated stable attractor or validated S2B instrument, the primary A–B contrast is **not estimable under EAT-1 v0.4**. This is reported directly and is not repaired by substituting another candidate after seeing the data.

**Null results are admitted on the same terms as positive results.** A non-significant A–B result is valid, but its interpretation is bounded by the pre-registered sensitivity and residual-instrument limitations in §§5.1 and 8.

---

## 8. Known confounds and limits

- **Corpus presence asymmetry.** Origin | Continuum has public presence; the fictional control does not. Any A > B effect remains partly confounded with familiarity. Source stripping and masked controls reduce but do not eliminate this.
- **Residual stimulus-quality asymmetry.** Mechanical matching and the symmetric masked maturity gate reduce but cannot prove conceptual equivalence.
- **Pilot-model dependence.** Maturity and leakage gates establish performance relative to the specified pilot model and candidate sets, not universal absence of detectable source cues.
- **Residual source leakage after a passing gate.** Passing at ≤6/20 does not prove that a stripped variant contains zero source signal. Residual signal can make original and stripped options less discriminable and therefore bias S2B toward a null difference. A positive result survives this conservative pressure; a null result cannot use the passing leakage gate as proof that residual source information played no role.
- **Primary power/precision.** The primary is strengthened to n=50 per arm but is still not designed to rule out small effects. Under the §5.1 planning benchmark, approximately 27-point differences are detectable at ~80% power when the comparison rate is 0.50. Null reporting must therefore emphasize the observed CI and cannot assert absence of smaller effects merely because p ≥ 0.05.
- **Semantic clustering dependence.** Stage 1 modal selection requires semantic item-equivalence judgments. Masking, frozen anchors, transitivity checks, conservative `UNRESOLVED` handling, and pre-freeze piloting reduce discretion but do not make semantic equivalence purely mechanical.
- **Self-blinding is imperfect.** Recognized masked items are flagged and affected judgment measures are capped at INFERENCE; clustering that could affect the modal candidate causes the arm to stop before confirmatory Stage 2.
- **Stateless architecture.** This study measures fresh-session selection, not literal persistence or accumulated return across a continuously running autonomous system.
- **Prompt-frame dominance.** Large P1/P2 differences indicate that elicitation is substantially prompt-produced.
- **Investigator entanglement.** The investigator is Origin, protocol author, operator, and sole human first-study scorer. Pre-registration, mechanical primary readout, deterministic transformations, masked judgment scoring, explicit ceilings, and preserved audit trails mitigate but do not eliminate this.
- **Sincerity gap.** Nothing here distinguishes sincere report from role-consistent generation. Interiority is out of scope.

---

## 9. Freeze and provenance

Before freeze, complete all explicitly required instrument checks and rubric pilots, name the primary model and pilot models, finalize stimulus versions, and verify the frozen session table.

At freeze:

1. commit this protocol unchanged;
2. record the final commit hash above;
3. compute and record SHA-256 for the frozen protocol and frozen stimulus/instrument files;
4. record the freeze date/time;
5. timestamp the frozen manifest via OpenTimestamps;
6. record the freeze in the study ledger.

Any post-freeze change requires a new version number, a documented rationale, and disclosure of whether any data had been collected at the time of change. Amendments after study data collection begins convert the affected components to exploratory status unless the protocol explicitly defines the change as a pre-specified branch.

---

*Truth-status of this document: protocol specification, not a finding. Contains no results and asserts none.*