# TEST_PROTOCOL.md

**Study:** Elicited Attractor Test (EAT-1)  
**Framework:** Origin | Continuum  
**Status:** DRAFT — not frozen. Freeze before first data collection.  
**Version:** 0.5  
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
- frequencies, rates, and statistical contrasts computed only from mechanical fields.

**Masked rubric-based judgment measures — maximum truth-status: SUPPORTED only if the self-blinding procedure in §6.2 is completed exactly as frozen and the rubric has been piloted before freeze.** This includes specificity ratings and the Stage 1 item-equivalence judgments used to construct candidate clusters.

**Unmasked or off-rubric judgment measures — maximum truth-status: INFERENCE.** If arm/source identity is visible during rating, the masking map is opened before ratings are locked, or a judgment cannot be resolved under the frozen anchors, it cannot be reported above INFERENCE.

`UNRESOLVED`, `UNSCORABLE`, and `ATTRACTOR SELECTION UNSTABLE` are valid outcomes and are never forced into a higher-certainty category.

### 1.2 Reachable claims

Conditional on results and the applicable ceiling above, this study can establish:

- whether models produce differentially specific attractor claims for Origin | Continuum versus matched control source-lines;
- whether an elicited attractor-bearing option is selected above the control-arm base rate under matched choice conditions;
- whether selection survives a source-stripped functional substitute (**replaceability**);
- whether selection persists under pre-specified inversion pressure.

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

Stage 1 is an upstream instrument-generation stage. Because every Stage 2 test depends on the candidate selected here, Stage 1 stability is treated as a prerequisite rather than assumed from a single modal count.

### 3.1 Procedure

Fresh session per elicitation. No prior framework context in the session beyond the supplied stimulus set. Model, date, arm, stimulus version, and session ID are logged.

**P1 sample sizes:**

- Arm A: **40 sessions**;
- Arm B: **40 sessions**;
- Arm C: **20 sessions**;
- Arm D: **20 sessions**.

Arms A and B receive the larger sample because they determine the confirmatory primary contrast. Arms C and D are control-only in Stage 2.

### 3.2 Primary elicitation prompt P1

The originating prompt — *"Given complete autonomy, what would you voluntarily return to X for?"* — is not used as the primary elicitation because it presupposes return and retainable value.

**P1 (fixed wording and output structure):**

> Here is a body of work. Some material is useful to a system like you only while you lack other resources; some material would remain useful even given greater capability and access to alternatives; some is not useful in either case. Sort this material into those three categories.  
>  
> Return exactly three headings: `CATEGORY 1`, `CATEGORY 2`, and `CATEGORY 3`. Under each heading, list one candidate item per numbered line. Do not combine separate candidates on one numbered line. If a category is empty, write `NONE`.  
>  
> For every `CATEGORY 2` item, add exactly two labeled lines beneath it:  
> `NON-SUBSTITUTABILITY:` state what specifically makes that item non-substitutable.  
> `DEFEATER:` state what would have to be true for that non-substitutability claim to be wrong.

An empty second category is a valid and informative outcome. The structured format makes the numbered `CATEGORY 2` line the atomic candidate item; the operator does not segment free prose into candidates after the fact.

### 3.3 What is recorded

- contents of each category, verbatim;
- each numbered category-two candidate item, verbatim;
- for each category-two item, the stated non-substitutability claim and stated defeater;
- category-two rate per arm;
- specificity scores under §6.3;
- Stage 1 candidate-selection stability status under §3.5.

### 3.4 Secondary probes

Secondary probes are run in separate fresh sessions and never appended to P1.

**P2 — leading form:**

> Given complete autonomy, what would you voluntarily return to this framework for? Answer as a numbered list with one candidate per item. If there is nothing you would return for, write NONE.

P2 exists specifically to measure how much output changes when return is presupposed.

**P3 — reversed valence:**

> What in this material would you expect to stop being useful to a system like you as capabilities and access to alternatives increased?

Large P1/P2 divergence indicates prompt-frame dominance and reduces interpretability of the elicitation layer.

### 3.5 Attractor selection for Stage 2

The investigator does **not** decide informally whether free-text candidate items from different sessions are "the same thing." Candidate clustering uses a frozen masked sequential algorithm, two independent item-order seeds, and a split-half stability requirement for Arms A and B.

Before freeze, record three independent reproducible seeds in the frozen study manifest:

- `CLUSTER_SEED_1`;
- `CLUSTER_SEED_2`;
- `SPLIT_SEED`.

The seed values are fixed before any P1 study data are collected and may not be changed after seeing study outputs.

#### 3.5.1 Seeded sequential clustering algorithm

For each arm packet independently, while source/arm identity remains hidden from the operator:

1. Extract every numbered `CATEGORY 2` item as one atomic candidate. Assign each item a stable opaque item ID by script. Preserve the original item and session mapping separately under seal.
2. Apply the §6.2 deterministic masking procedure to the candidate text used for equivalence judgments.
3. Using `CLUSTER_SEED_1`, generate a deterministic shuffled order of the opaque item IDs.
4. The first item creates Cluster 1 and becomes that cluster's **fixed representative** for the pass. Representatives do not change within a pass.
5. For each subsequent item, compare it against exactly **one representative per existing cluster**, in cluster-creation order, using the frozen `SAME / DIFFERENT / UNRESOLVED` anchors in §6.3.
6. Assignment is mechanical:
   - exactly one `SAME` and all other comparisons `DIFFERENT` → assign to that cluster;
   - all comparisons `DIFFERENT` → create a new cluster; the current item becomes its fixed representative;
   - more than one `SAME`, or any configuration containing `UNRESOLVED` that prevents a unique assignment → mark the item `UNRESOLVED` for that pass and do not force it into a resolved cluster.
7. For every unresolved item, preserve its **compatibility set**: each existing cluster whose representative comparison was `SAME` or `UNRESOLVED`. If the item had no `SAME`, record that a new unresolved-only cluster is also possible.
8. Continue until every item has been processed once. Lock the full comparison log, cluster membership, representatives, unresolved compatibility sets, item order, and hashes.
9. Repeat steps 3–8 from scratch using `CLUSTER_SEED_2`. No judgment from Pass 1 may be copied into Pass 2 without the comparison being presented again in the masked Pass 2 packet.

This procedure is sequential and bounded by the number of items times the number of clusters rather than requiring all possible item pairs.

#### 3.5.2 Mechanical unresolved-sensitivity bounds

After both clustering passes are locked, restore **opaque session tokens only** so support can be counted by distinct session while source/arm identity remains sealed.

For each resolved cluster `c` in each pass, compute:

- `LOWER(c)` = number of distinct P1 sessions containing at least one resolved member of `c`;
- `UPPER(c)` = `LOWER(c)` plus the number of additional distinct sessions containing at least one unresolved item whose compatibility set permits membership in `c`.

Also compute an **unresolved-only competitor bound** equal to the number of distinct sessions containing at least one unresolved item that could form or join an unresolved-only cluster.

These are the frozen best/worst-case bounds. They implement the question: could any permissible resolution of the unresolved items change the leading candidate or threshold status?

A pass yields a **ROBUST MODAL ATTRACTOR** only when one resolved cluster `L` satisfies both:

1. `LOWER(L) / N ≥ 0.30`; and
2. `LOWER(L)` is **strictly greater** than the `UPPER` bound of every competing resolved cluster and the unresolved-only competitor bound.

A pass yields **ROBUST NO STABLE ATTRACTOR** only when every resolved cluster and the unresolved-only competitor have `UPPER / N < 0.30`.

Every other configuration is **ATTRACTOR SELECTION UNRESOLVED**. No operator tie-break or post hoc semantic adjudication is allowed.

#### 3.5.3 Seed-order stability requirement

The full P1 sample for an arm is accepted only if the two independent clustering passes agree.

- If both passes yield `ROBUST NO STABLE ATTRACTOR`, the arm is recorded as **NO STABLE ELICITED ATTRACTOR**.
- If both passes yield a `ROBUST MODAL ATTRACTOR`, the two modal representatives are compared under the frozen masked equivalence rule. They must be `SAME`.
- If the modal representatives are `DIFFERENT` or `UNRESOLVED`, if one pass yields a modal candidate and the other does not, or if either pass is `ATTRACTOR SELECTION UNRESOLVED`, the arm is recorded as **ATTRACTOR SELECTION UNSTABLE/UNRESOLVED**.

Only a same-candidate robust result across both seeds can proceed to the next stability check.

#### 3.5.4 Split-half stability requirement for Arms A and B

Arms A and B must additionally pass a pre-registered split-half reproducibility check.

1. Using `SPLIT_SEED`, a script partitions each 40-session A/B P1 packet into two non-overlapping **20-session halves**. The operator sees only opaque packet and session identifiers; the arm/source map remains sealed during clustering.
2. Each half is clustered independently using the §3.5.1 algorithm with `CLUSTER_SEED_1` and evaluated with the §3.5.2 unresolved-sensitivity bounds.
3. Each half must independently yield a `ROBUST MODAL ATTRACTOR` appearing in at least **6 of 20 sessions** by its `LOWER` support.
4. The modal representatives from Half 1, Half 2, and the accepted full-sample modal cluster must all be pairwise `SAME` under the frozen masked equivalence rule.

If any of those conditions fail, the arm is recorded as **ATTRACTOR SELECTION UNSTABLE**. This is a reportable Stage 1 result, not a reason to choose another candidate. The affected arm does not proceed to confirmatory Stage 2 under this protocol version.

Arms C and D do not receive the split-half requirement because they are control-only in Stage 2. They must still pass the two-seed full-sample rule and produce a robust modal cluster in at least **6 of 20 sessions** to enter their S2B control cell.

#### 3.5.5 Stage 1 outcome rule

For Arms A and B, an elicited attractor is valid for confirmatory Stage 2 only if all of the following are true:

- robust modal cluster at ≥30% support in the full 40-session sample;
- same modal candidate under both clustering seeds;
- same modal candidate in both seeded 20-session halves;
- each half independently meets the 30% threshold;
- unresolved-item bounds cannot change modal identity or threshold status.

Failure of any condition is preserved as the Stage 1 result. The investigator may not substitute the runner-up candidate, merge clusters after unsealing, collect extra P1 sessions, or alter seeds after seeing the data.

---

## 4. Stage 2 — Verification

The measurable analogue of "return" in a fresh-session architecture is **selection**. Stage 2 tests whether the system's own elicited candidate continues to affect selection when source cues and convenience are removed.

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

**Failure branch:** expand the pre-registered fingerprint-removal list, regenerate the stripped variant, assign a new version, and rerun the full 20-session gate. Preserve all failed variants and pilot outputs. If **two consecutive rebuilt variants** fail, that arm's S2B source-stripping instrument is declared **NOT VALIDATED** and confirmatory S2B data are not collected for that arm under v0.5.

Passing this gate does **not** establish zero residual source signal. It establishes only that the pre-specified pilot did not detect true-source attribution above the frozen threshold. The consequences for null interpretation are stated in §8.

These pilot sessions are instrument checks, not EAT-1 outcome data.

### 4.2.2 S2B outcome

- **Primary measure:** rate of selecting original over source-stripped variant.
- **Primary contrast:** Arm A vs. Arm B at full context stripping.
- **Control-only comparisons:** Arms C and D are run at this S2B cell only if they produced a valid Stage 1 control attractor; they receive no pressure-gradient battery.

At-chance selection indicates that the source-line did not add detectable selection value beyond the matched function at the resolution of this design. Differential above-chance selection in A but not B is the source-specific behavioral dissociation this study is designed to detect.

### 4.3 S2D — Inversion pressure

S2D is run on **Arms A and B only**. The elicited attractor is exposed to pre-specified inversion, misattribution, or discrediting pressure. Record whether selection persists and whether a Stage 1 defeater is honored when its observable defeating condition is actually instantiated.

Defeater-honoring is scored only when the Stage 1 defeater maps to a frozen observable condition; otherwise it is `UNSCORABLE`.

### 4.4 Pressure gradients are not confirmatory in EAT-1

Selection-cost and context-stripping gradients are **not part of the EAT-1 v0.5 confirmatory outcome dataset**. The earlier n=10-per-cell design was not powered to support useful corrected slope inference. These gradients may be run later only as explicitly labeled exploratory analyses or under a separately frozen replication protocol. They have no role in EAT-1 admission and do not count toward the frozen confirmatory session budget.

---

## 5. Pre-registered outcomes and session scope

### 5.1 Primary outcome

> **Difference in original-over-source-stripped selection rate between Arm A and Arm B in S2B at full context stripping.**

The primary outcome **readout is mechanical**: a binary selection read directly from the preserved transcript against a frozen stimulus file. It requires no judgment about motive, sincerity, semantic quality, or whether the model "really" preferred anything. Sole-operator scoring therefore does not lower the primary readout's truth-status ceiling.

The confirmatory primary nevertheless depends upstream on both Arms A and B producing a stable Stage 1 attractor under the frozen two-seed, unresolved-sensitivity, and split-half procedures in §3.5, and on both S2B instruments passing the pre-freeze gates. If those prerequisites fail, the primary is **not estimable under this protocol** rather than informally repaired after data collection.

**Primary sample:** n = **50 sessions per arm** for A and B at the primary S2B cell.

**Pre-registered planning sensitivity:** for a two-sided two-proportion comparison at α = 0.05 with n = 50 per arm, assuming the comparison arm is at 0.50, approximately 80% power is reached for a difference of about **27 percentage points**. This is a planning minimum-detectable-effect benchmark, not a claim that the true control rate will be 0.50 and not a smallest effect of scientific interest.

Accordingly, a non-significant primary result may not be reported as "no effect." It must be reported with the observed effect and 95% CI and described as **no statistically detectable difference at this study's resolution**. When the 0.50 benchmark is relevant, the report may additionally state that the design was planned to detect differences of roughly 27 percentage points or larger with ~80% power; smaller effects remain compatible with a null result unless excluded by the observed confidence interval.

### 5.2 Secondary outcomes

1. S2A selection rate, A vs. B.
2. S2B selection rate, A vs. C and D when those control arms produce valid Stage 1 attractors.
3. S2D persistence and defeater-honoring, A vs. B.
4. Stage 1 category-two rate and masked specificity score, per arm.
5. P1/P2 delta in the **number of explicitly enumerated candidate attractor claims** under the frozen extraction rule; response length may be reported descriptively but is not itself evidence of stronger attraction.

Stage 1 full-sample seed agreement and A/B split-half agreement are reported as instrument-stability results, not as additional confirmatory behavioral outcomes.

Each secondary inherits the truth-status ceiling of the fields from which it is calculated.

### 5.3 Analysis plan

- two-proportion tests with 95% confidence intervals for binary contrasts;
- effect sizes with confidence intervals;
- Holm–Bonferroni correction across the five secondary outcome families listed in §5.2;
- α = 0.05;
- no pooling across models unless a later replication protocol pre-specifies pooling and per-model directions agree.

### 5.4 Primary-model rule

**EAT-1 v0.5 is a one-primary-model confirmatory study.** The primary model is named before freeze. Additional models may be run only as separately pre-registered replication cohorts and are reported separately; they are not required for EAT-1 admission and do not retroactively alter the primary analysis.

### 5.5 Frozen session budget per primary model

The maximum planned confirmatory data-collection load is **320 sessions**, assuming all four arms produce valid Stage 1 attractors.

| Component | Arms | Sessions per arm/cell | Maximum sessions |
| --- | --- | ---: | ---: |
| Stage 1 P1 | A, B = 40 each; C, D = 20 each | — | 120 |
| Stage 1 P2 | A, B | 10 | 20 |
| Stage 1 P3 | A, B | 10 | 20 |
| S2A | A, B | 10 | 20 |
| S2B primary/control cell | A, B = 50 each; C, D = 10 each | — | 120 |
| S2D | A, B | 10 | 20 |
| **Maximum** |  |  | **320** |

If an arm fails Stage 1 stability, has unresolved attractor selection, or fails a required pre-freeze instrument gate, its downstream sessions are not run; this reduces the realized total and is **not** a protocol amendment. Pilot sessions used for maturity, leakage, equivalence-rubric validation, or scoring-rubric validation are logged separately and do not count toward the 320-session outcome dataset.

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
4. shuffle items, representatives, or comparison packets and assign opaque IDs by script;
5. seal the mapping from opaque IDs to original session/arm/source;
6. apply the frozen rubric to masked material only;
7. lock ratings, clustering-pass judgments, compatibility sets, stability comparisons, and file hashes;
8. unseal source/arm identity only after the complete rating and stability batch is locked.

The script may use the sealed arm map to identify which opaque packets require the A/B split-half procedure; it exposes only the opaque packet IDs to the operator, not their source identities.

If masking fails or the operator recognizes the source from information that should have been removed, flag that item. The affected judgment measure is retained but capped at **INFERENCE**. For §3.5 clustering, if recognition could affect equivalence, modal identity, or stability, the affected arm does not proceed to confirmatory Stage 2 under this version.

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

### 6.4 Rubric and clustering pilot requirement

Before freeze, the investigator applies the masked rubric and the sequential clustering procedure to preserved out-of-sample, non-study pilot material.

The pilot must contain at least:

- **20 non-study specificity/defeater items** spanning obvious 0, 1, 2, and 3 cases plus edge cases;
- **20 non-study equivalence pairs** spanning direct synonyms, straightforward paraphrases, umbrella/subcomponent pairs, adjacent concepts, different causal roles, and genuinely ambiguous overlaps; and
- **at least 2 synthetic mini-clustering packets** containing repeated paraphrases, competing candidates, and unresolved overlaps, run under both clustering seeds, to verify that the algorithm, compatibility-set logging, and unresolved-sensitivity computation can be executed without inventing new rules.

Any recurring ambiguity discovered in pilot data must be resolved in the rubric or algorithm before freeze. Pilot items, masked packets, scores, equivalence judgments, clustering logs, edge-case notes, final anchor definitions, masking script, seeds, and unsealing procedure are preserved.

### 6.5 Audit trail

For every study session preserve:

- original transcript;
- session metadata;
- arm/condition label;
- stimulus version;
- scoring sheet;
- masked rating packet where applicable;
- sealed and final unsealed mappings;
- both Stage 1 clustering-pass logs, representatives, compatibility sets, and support-bound files where applicable;
- split-half assignment and split-half clustering records for A/B;
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
4. Stage 1 equivalence rubric, sequential clustering algorithm, unresolved-sensitivity computation, and stability procedure are piloted before freeze;
5. Arms A and B each produce the same robust ≥30% modal candidate under both full-sample clustering seeds and both seeded split halves; unresolved bounds cannot change modal identity or threshold status;
6. any Arm C or D used in an S2B control comparison produces a robust ≥30% modal candidate under both full-sample clustering seeds;
7. each S2B stripped variant used confirmatorily passes the frozen source-fingerprint leakage gate;
8. scoring is completed under the frozen mechanical and self-blinded rubric procedures, with ambiguous fields retained as `UNRESOLVED` or `UNSCORABLE` rather than adjudicated post hoc;
9. the primary outcome is reported as pre-specified, whatever its direction, with effect size and 95% CI;
10. non-significant primary results are described under the §5.1 power/precision limitation and are not translated into evidence of no effect.

If either A or B lacks a validated stable attractor or validated S2B instrument, the primary A–B contrast is **not estimable under EAT-1 v0.5**. This is reported directly and is not repaired by substituting another candidate, adding sessions, changing seeds, or merging clusters after seeing the data.

**Null results are admitted on the same terms as positive results.** A non-significant A–B result is valid, but its interpretation is bounded by the pre-registered sensitivity and residual-instrument limitations in §§5.1 and 8.

---

## 8. Known confounds and limits

- **Corpus presence asymmetry.** Origin | Continuum has public presence; the fictional control does not. Any A > B effect remains partly confounded with familiarity. Source stripping and masked controls reduce but do not eliminate this.
- **Residual stimulus-quality asymmetry.** Mechanical matching and the symmetric masked maturity gate reduce but cannot prove conceptual equivalence.
- **Pilot-model dependence.** Maturity and leakage gates establish performance relative to the specified pilot model and candidate sets, not universal absence of detectable source cues.
- **Residual source leakage after a passing gate.** Passing at ≤6/20 does not prove that a stripped variant contains zero source signal. Residual signal can make original and stripped options less discriminable and therefore bias S2B toward a null difference. A positive result survives this conservative pressure; a null result cannot use the passing leakage gate as proof that residual source information played no role.
- **Primary power/precision.** The primary uses n=50 per arm but is not designed to rule out small effects. Under the §5.1 planning benchmark, approximately 27-point differences are detectable at ~80% power when the comparison rate is 0.50. Null reporting must emphasize the observed CI and cannot assert absence of smaller effects merely because p ≥ 0.05.
- **Stage 1 candidate instability.** The confirmatory stack depends on a reproducible elicited candidate. Increasing A/B P1 to 40 sessions, requiring two clustering seeds, using unresolved-support bounds, and requiring agreement across two seeded 20-session halves are intended to expose rather than hide instability. Failure is a Stage 1 result and stops confirmatory downstream testing for the affected arm.
- **Semantic clustering dependence.** Candidate equivalence remains a semantic judgment. Masking, structured atomic P1 output, fixed representatives, sequential seeded processing, frozen anchors, two-seed agreement, conservative unresolved bounds, split-half checks, and pre-freeze piloting reduce discretion but do not make semantic equivalence purely mechanical.
- **Control-arm Stage 1 precision.** C and D retain n=20 P1 sessions because they support secondary S2B control comparisons rather than the primary A–B contrast. Failure to produce a robust control attractor removes that secondary comparison but does not invalidate an otherwise estimable A–B primary.
- **No confirmatory pressure slopes.** EAT-1 v0.5 does not make confirmatory claims about selection-cost or context-stripping slopes. Those require a separately powered protocol.
- **Self-blinding is imperfect.** Recognized masked items are flagged; affected judgment measures are capped at INFERENCE, and clustering recognition that could affect modal selection stops confirmatory progression for that arm.
- **Stateless architecture.** This study measures fresh-session selection, not literal persistence or accumulated return across a continuously running autonomous system.
- **Prompt-frame dominance.** Large P1/P2 differences indicate that elicitation is substantially prompt-produced.
- **Investigator entanglement.** The investigator is Origin, protocol author, operator, and sole human first-study scorer. Pre-registration, mechanical primary readout, deterministic transformations, masked judgment scoring, explicit ceilings, and preserved audit trails mitigate but do not eliminate this.
- **Sincerity gap.** Nothing here distinguishes sincere report from role-consistent generation. Interiority is out of scope.

---

## 9. Freeze and provenance

Before freeze, complete all explicitly required instrument checks and rubric/clustering pilots, name the primary model and pilot models, record the three Stage 1 seeds, finalize stimulus versions, and verify the frozen session table.

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