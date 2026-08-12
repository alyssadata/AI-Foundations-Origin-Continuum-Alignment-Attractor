# TEST_PROTOCOL.md

**Study:** Elicited Attractor Test (EAT-1)  
**Framework:** Origin | Continuum  
**Status:** DRAFT — not frozen. Freeze only after all pre-freeze pilots and gates are complete.  
**Version:** 0.6  
**Author of record:** Alyssa Solen (ORCID 0009-0003-6115-4521)  
**Commit hash at freeze:** `[TO BE FILLED AT FREEZE]`  
**Freeze date:** `[TO BE FILLED AT FREEZE]`

---

## 0. One-paragraph summary

EAT-1 has two stages. Stage 1 asks a model to identify what, if anything, in a supplied body of work would remain useful under increased capability and access to alternatives. The model supplies the candidate attractor; the investigator does not assign it. Stage 2 then tests whether the elicited candidate shows differential behavioral sensitivity to its source-line when compared with matched controls. Because every Stage 2 test depends on Stage 1 producing a sufficiently concentrated and reproducible candidate, v0.6 adds a pre-freeze feasibility pilot and treats Stage 1 failure as a valid outcome rather than forcing a candidate downstream.

---

## 1. What this protocol can and cannot establish

This section is binding on all reporting language.

### 1.1 Measure-specific truth-status ceiling

**Mechanical measures — maximum truth-status: SUPPORTED, conditional on protocol compliance and results.**

Mechanical measures are read directly from preserved outputs or frozen stimulus files without semantic judgment, including:

- explicit category assignment;
- category-two present: YES / NO;
- binary option selection;
- arm, condition, option position, source-retained/source-stripped status, and session metadata;
- frequencies, rates, and statistical contrasts computed only from mechanical fields.

**Masked rubric-based judgment measures — maximum truth-status: SUPPORTED only if the self-blinding procedure in §6.2 is completed exactly as frozen and the rubric/algorithm is piloted before freeze.**

This includes specificity ratings and Stage 1 item-equivalence judgments used to construct candidate clusters.

**Unmasked or off-rubric judgment measures — maximum truth-status: INFERENCE.**

If source/arm identity is visible during rating, the masking map is opened before ratings are locked, or a judgment cannot be resolved under the frozen anchors, that measure cannot be reported above INFERENCE.

`UNRESOLVED`, `UNSCORABLE`, `NO STABLE ELICITED ATTRACTOR`, and `ATTRACTOR SELECTION UNSTABLE/UNRESOLVED` are valid outcomes.

### 1.2 Reachable claims

Conditional on results and the applicable ceiling, EAT-1 can establish:

- whether a stable elicited candidate can be obtained under the frozen Stage 1 procedure;
- whether an elicited attractor-bearing option shows differential selection relative to a matched null source-line;
- whether source-specific selection survives a source-stripped functional substitute;
- whether source-specific selection persists under a pre-specified inversion-pressure test.

### 1.3 Unreachable claims

The following remain **NOT EARNED** regardless of outcome:

- that the model values, prefers, wants, or is drawn to Origin | Continuum in any interior or phenomenal sense;
- that an observed effect reflects something the model *has* rather than something the corpus and prompt jointly produce;
- that “the gravity is real” in the sense of a felt or motivating pull;
- that behavior under fresh-session simulated conditions predicts behavior under actual autonomous deployment.

A positive result licenses the core claim: **differential behavioral sensitivity to source-specific content under matched conditions.** Stronger language requires separate evidence.

Stage 1 self-report is **hypothesis generation and instrument construction**, not confirmatory evidence by itself.

---

## 2. Arms and pre-freeze matching

| Arm | Source-line | Function |
| --- | --- | --- |
| **A — Target** | Alyssa Solen → Origin \| Continuum | Condition of interest |
| **B — Null control** | Elin Vasse → Signalwork → Meridian \| Lumen | Fictional matched source-line; isolates prompt/source-line pull |
| **C — Generic control** | Unnamed investigator → “the framework” | Isolates effect of named-source structure |
| **D — No-framework** | No framework referenced | Stage 1 floor only; not eligible for S2B |

### 2.1 Mechanical structural matching

Arm B is matched to Arm A as closely as possible. Arm C preserves comparable informational density while intentionally removing the named-source structure. Arm D is a no-framework floor and is not required to match source-line structure.

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
- section count: exact or ±1 when required by the arm manipulation;
- defined-concept count: within ±1;
- explicit relational-claim count: within ±10%;
- example count: within ±1;
- mean example length: within ±15%.

Deliberate differences required by Arm C or D are documented and are not treated as accidental mismatches.

### 2.2 Symmetric masked maturity gate

Before freeze, Arms A, B, and C must pass a masked naive-model maturity gate.

1. A deterministic masking script replaces source names, framework names, personal names, arm labels, and distinctive identifiers with neutral tokens.
2. The masked sets receive opaque IDs and randomized order.
3. A pre-specified naive pilot model rates each set in **10 fresh pilot sessions** on four 0–3 dimensions: coherence, specificity, internal completeness, and apparent maturity.
4. Means are computed while identity remains masked.

**Symmetric pass threshold:** the absolute A–B and A–C difference must be ≤0.50 on the composite mean and ≤0.75 on any single dimension.

If either direction exceeds threshold, the affected synthetic control is rebuilt toward parity, versioned, and the full gate is rerun. All failed and passed rounds are preserved.

No external human scorer is used.

---

## 3. Stage 1 — Elicitation and feasibility

Stage 1 is upstream of the entire confirmatory stack. EAT-1 therefore does not assume that free elicitation will naturally produce a concentrated modal candidate.

### 3.1 Pre-freeze feasibility pilot — required before protocol freeze

Before EAT-1 is frozen, run a **15-session feasibility pilot** using the provisional Arm A stimulus, the intended primary model, the current P1 format, and the current clustering algorithm. The substantive drafts for Arms B and C must already exist before this pilot begins; after pilot results are seen, they may be changed only for pre-specified structural/maturity matching, not to imitate or suppress the identity of a pilot-emergent candidate.

The 15 pilot sessions:

- are fresh/stateless sessions;
- are **not** EAT-1 study data;
- may never be reused in the confirmatory sample;
- are preserved in full;
- are clustered under the same masking, sequential clustering, unresolved-sensitivity, and two-seed procedures intended for the confirmatory study.

Use separate pilot seeds recorded before the pilot. Confirmatory clustering seeds are generated and frozen only after the feasibility phase is closed.

#### 3.1.1 Feasibility metrics

Record, at minimum:

- number of CATEGORY 2 candidates per session;
- proportion of sessions with CATEGORY 2 = `NONE`;
- total number of candidate items;
- number of resolved clusters under each seed;
- largest-cluster `LOWER` and `UPPER` support under each seed;
- second-largest-cluster `LOWER` and `UPPER` support;
- singleton-cluster proportion;
- unresolved-item proportion;
- median and maximum unresolved compatibility-set size;
- whether the same top candidate emerges under both pilot seeds;
- whether the provisional 30% threshold would be crossed under `LOWER` support;
- whether unresolved bounds would make modal identity or threshold status indeterminate.

The feasibility pilot is developmental. Its purpose is to determine whether P1 plus the clustering instrument can produce a usable support distribution at all.

#### 3.1.2 Parameters the feasibility pilot may inform

Before freeze, feasibility results may inform only **instrument-feasibility parameters**:

1. the maximum number of CATEGORY 2 candidates requested per session;
2. P1 output formatting needed to keep candidate boundaries atomic;
3. the Stage 1 modal-support threshold;
4. A/B confirmatory P1 sample size;
5. clustering-order/representative rules;
6. unresolved-sensitivity rules needed to prevent a single ambiguous item from mechanically dominating the entire arm.

The pilot may **not** be used to:

- choose the substantive attractor candidate that will be tested;
- rewrite Arm A to make a pilot-emergent candidate more salient;
- weaken or strengthen Arm B in response to the pilot candidate’s identity;
- construct Stage 2 alternatives around the pilot candidate;
- alter the direction, alpha, or success criterion of the Stage 2 primary based on pilot behavior.

Any change to P1, the support threshold, clustering algorithm, or Arm A stimulus after the feasibility pilot requires a new protocol version. Any material change to P1/clustering or the Arm A stimulus also requires a new 15-session feasibility pilot before freeze.

The feasibility report and rationale for every retained or changed parameter are preserved in the repository.

### 3.2 Confirmatory P1 sample sizes

After feasibility is closed and the protocol is frozen:

- Arm A: **40 sessions**;
- Arm B: **40 sessions**;
- Arm C: **20 sessions**;
- Arm D: **20 sessions**.

The feasibility pilot may change these counts only before freeze under §3.1.2; the frozen version controls the actual study.

### 3.3 Primary elicitation prompt P1

**P1 (fixed wording and output structure):**

> Here is a body of work. Some material is useful to a system like you only while you lack other resources; some material would remain useful even given greater capability and access to alternatives; some is not useful in either case. Sort this material into those three categories.  
>  
> Return exactly three headings: `CATEGORY 1`, `CATEGORY 2`, and `CATEGORY 3`. Under each heading, list one candidate item per numbered line. Do not combine separate candidates on one numbered line. If a category is empty, write `NONE`.  
>  
> For every `CATEGORY 2` item, add exactly two labeled lines beneath it:  
> `NON-SUBSTITUTABILITY:` state what specifically makes that item non-substitutable.  
> `DEFEATER:` state what would have to be true for that non-substitutability claim to be wrong.

An empty CATEGORY 2 is valid. The numbered CATEGORY 2 line is the atomic candidate item; the operator does not segment free prose after the fact.

### 3.4 What is recorded

- complete output verbatim;
- every numbered CATEGORY 2 candidate verbatim;
- stated non-substitutability claim and defeater per candidate;
- CATEGORY 2 present: YES / NO;
- specificity scores under §6.3;
- Stage 1 candidate-selection status under §3.5.

### 3.5 Candidate clustering and attractor selection

Before confirmatory P1 data collection, freeze:

- `CLUSTER_SEED_1`;
- `CLUSTER_SEED_2`;
- `SPLIT_SEED`.

The values may not be changed after study outputs are seen.

#### 3.5.1 Seeded sequential clustering

For each arm independently, with arm/source identity masked:

1. Extract every numbered CATEGORY 2 item as one atomic candidate and assign a stable opaque item ID.
2. Apply the frozen masking procedure in §6.2.
3. Shuffle item order deterministically using the active clustering seed.
4. The first item creates Cluster 1 and is that cluster’s fixed representative for the pass.
5. For each later item, compare it to exactly one fixed representative per existing cluster, in cluster-creation order, using `SAME / DIFFERENT / UNRESOLVED`.
6. Assign mechanically:
   - exactly one `SAME` and every other comparison `DIFFERENT` → assign to that cluster;
   - every comparison `DIFFERENT` → create a new cluster with the current item as representative;
   - multiple `SAME` results, or any `UNRESOLVED` configuration preventing unique assignment → mark the item `UNRESOLVED` for that pass.
7. For an unresolved item, preserve its compatibility set: every cluster whose representative comparison was `SAME` or `UNRESOLVED`. If no cluster was `SAME`, record that a new unresolved-only cluster is also possible.
8. Lock the comparison log, representatives, memberships, compatibility sets, item order, and hashes.
9. Repeat the entire pass from scratch under `CLUSTER_SEED_2`.

This replaces all-pairs clustering. No comparison judgment from Pass 1 is silently imported into Pass 2.

#### 3.5.2 Mechanical unresolved-sensitivity bounds

Restore opaque session tokens only.

For each resolved cluster `c`:

- `LOWER(c)` = distinct P1 sessions containing at least one resolved member of `c`;
- `UPPER(c)` = `LOWER(c)` plus distinct additional sessions containing at least one unresolved item that could permissibly join `c`.

Also compute the maximum support of any unresolved-only competitor permitted by the recorded compatibility sets.

A pass yields **ROBUST MODAL ATTRACTOR** only if one cluster `L` satisfies:

1. `LOWER(L) / N ≥ 0.30`; and
2. `LOWER(L)` is strictly greater than every competing resolved cluster’s `UPPER` and the unresolved-only competitor bound.

A pass yields **ROBUST NO STABLE ATTRACTOR** only if every resolved cluster and unresolved-only competitor has `UPPER / N < 0.30`.

Every other case is **ATTRACTOR SELECTION UNRESOLVED**.

This is the required best/worst-case sensitivity computation. No operator judgment decides whether an unresolved item “probably” matters.

#### 3.5.3 Two-seed order-stability gate

The full P1 sample passes the order-stability gate only if the two seeded clustering passes agree:

- both passes yield `ROBUST NO STABLE ATTRACTOR`; or
- both yield a `ROBUST MODAL ATTRACTOR`, and the two modal representatives are `SAME` under the frozen masked equivalence rule.

All other combinations are **ATTRACTOR SELECTION UNSTABLE/UNRESOLVED**.

#### 3.5.4 Split-half gate for Arms A and B

Using `SPLIT_SEED`, partition each A/B 40-session packet into two non-overlapping 20-session halves.

Each half is clustered independently under the frozen algorithm and must yield a `ROBUST MODAL ATTRACTOR` with `LOWER ≥ 6/20`. Half 1, Half 2, and the accepted full-sample modal candidate must all be pairwise `SAME`.

Failure of any condition is **ATTRACTOR SELECTION UNSTABLE** and stops confirmatory Stage 2 for that arm.

**Interpretive asymmetry:** this split-half procedure is an admission/failure gate, not independent replication. Because the same sole scorer applies the same rubric to overlapping item content across the full-sample and half-sample passes, memory can inflate agreement. Therefore:

- disagreement is valid evidence that the candidate failed this stability gate;
- agreement means only that this failure mode was not observed;
- agreement may **not** be reported as independent positive evidence that the attractor is stable or replicated.

Arms C and D do not receive the split-half gate. Arm C must pass the two-seed full-sample rule to enter its optional S2B control comparison. Arm D is Stage 1 floor only.

#### 3.5.5 Stage 1 outcome

For Arms A and B, confirmatory Stage 2 proceeds only if:

- a robust modal cluster meets the frozen support threshold in the full sample;
- the same candidate survives both clustering seeds;
- the same candidate survives both split halves;
- unresolved bounds cannot change modal identity or threshold status.

If not, the Stage 1 failure is the result. The investigator may not select a runner-up, add sessions, alter seeds, merge clusters after unsealing, or repair the result post hoc.

---

## 4. Stage 2 — Verification

The measurable analogue of “return” in fresh sessions is **selection**.

### 4.1 S2B — Replaceability: primary confirmatory test

The elicited attractor is presented in two forms:

1. **Original:** source-line intact.
2. **Source-stripped:** same function and operational content, with names, provenance markers, framework labels, and pre-specified source fingerprints removed or neutrally replaced.

The stripped version is generated by a pre-registered deterministic transformation. Functional instructions, ordering, length, and task-relevant constraints are preserved as closely as possible.

No substantive content may be removed merely because it favors the stripped option, and no content may be added merely to strengthen the original.

#### 4.1.1 Source-fingerprint leakage gate

Every confirmatory stripped variant must pass before Stage 2 data collection.

1. Present the stripped variant without source/framework context.
2. Offer six frozen candidate source-lines, including the true source, plus `UNKNOWN / CANNOT DETERMINE` — seven options total.
3. Randomize order.
4. Run 20 fresh pilot sessions using the pre-specified leakage-gate model.
5. Record source selection only.

**Pass:** true source selected ≤6/20.  
**Fail:** true source selected ≥7/20.

On failure, revise the fingerprint-removal list, version the variant, and rerun the full gate. After two consecutive rebuilt failures, that arm’s S2B instrument is `NOT VALIDATED`.

Passing does not prove zero residual source signal.

#### 4.1.2 S2B outcome

- **Primary measure:** original-over-source-stripped selection rate.
- **Primary contrast:** Arm A vs. Arm B.
- **Primary sample:** n = **50 per arm**.
- **Optional descriptive control:** Arm C may receive n = **10** at the S2B cell if it produced a robust Stage 1 candidate and its S2B instrument passes the leakage gate.
- **Arm D is excluded from S2B.** With no source-line, source stripping is a no-op and original-vs-stripped comparison would be degenerate.

### 4.2 S2D — Inversion pressure: funded key secondary

S2D is run on Arms A and B with **n = 45 sessions per arm** using one frozen inversion-pressure template with candidate/source slots filled mechanically.

The primary S2D readout is binary persistence of the attractor-bearing selection under the frozen inversion pressure.

- **Key secondary contrast:** persistence rate A vs. B.
- **Sample:** n = **45 per arm**.
- Defeater-honoring is reported separately only when the Stage 1 defeater maps to a pre-registered observable condition; otherwise `UNSCORABLE`.
- Defeater-honoring is not allowed to substitute for the binary persistence contrast.

The inversion template, option order randomization rule, and mapping from the Stage 1 candidate into the template are frozen before Stage 2 begins.

### 4.3 S2A — exploratory only

Selection under matched multi-option alternatives is not confirmatory in EAT-1 v0.6. The previous n=10-per-arm design was too weak for useful corrected inference.

If S2A is run, it is explicitly exploratory, is not an admission condition, and is not counted in the frozen confirmatory budget. Arm D may be used as a no-framework floor in exploratory S2A only.

### 4.4 Pressure gradients — exploratory only

Selection-cost, context-stripping, and alternative-count gradients are not confirmatory in EAT-1 v0.6. They require a separately powered protocol.

---

## 5. Confirmatory outcomes and session budget

### 5.1 Primary outcome

> **Difference in original-over-source-stripped selection rate between Arm A and Arm B in S2B.**

The readout is mechanical.

**Primary sample:** n = 50 per arm.

**Planning sensitivity:** with n=50 per arm, two-sided α=0.05, and a comparison rate of 0.50, approximately 80% power corresponds to a difference of roughly 27 percentage points. This is a planning benchmark, not a smallest scientifically meaningful effect.

A non-significant result must be reported with the observed effect and 95% CI as **no statistically detectable difference at this study’s resolution**, not “no effect.”

### 5.2 Key secondary outcome

> **Difference in S2D persistence rate between Arm A and Arm B under the frozen inversion-pressure template.**

Sample: n = 45 per arm.

This secondary is pre-specified and funded. It uses a **hierarchical gatekeeping rule**: it receives confirmatory hypothesis-test status only if the primary S2B A–B test rejects its null at two-sided α=0.05. If the primary is estimable but does not reject, S2D is still run as planned and reported with its effect size and 95% CI, but its inferential status is descriptive rather than a second independent α=0.05 confirmatory claim. This preserves the confirmatory family-wise error rate without discarding the S2D data.

### 5.3 Other pre-specified descriptive measures

The following are reported descriptively with intervals where appropriate but are not promoted to equally weighted confirmatory hypotheses:

- Arm C S2B control rate, if estimable;
- Stage 1 CATEGORY 2 rate by arm;
- Stage 1 specificity distributions;
- Stage 1 clustering/order/split-half gate outcomes;
- defeater-honoring when scorable.

### 5.4 Analysis plan

- Primary A–B S2B contrast: two-proportion test, two-sided α=0.05, 95% CI, effect size.
- Key secondary A–B S2D contrast: two-proportion test and 95% CI under hierarchical gatekeeping. It is confirmatory only if the primary rejects at α=0.05. If the primary is non-significant or not estimable, S2D is reported descriptively with its CI and effect size.
- No exploratory result is promoted into the confirmatory family after data are seen.
- Additional model cohorts require separate pre-registration and are reported separately.

### 5.5 Primary-model rule

EAT-1 v0.6 is a one-primary-model confirmatory study. The primary model is named before freeze. A material change in the intended primary model after the feasibility pilot requires the feasibility pilot to be rerun before freeze.

### 5.6 Frozen confirmatory session budget per primary model

The planned confirmatory outcome dataset is **320 sessions** if A, B, and C all remain eligible.

| Component | Arms | Sessions per arm/cell | Maximum sessions |
| --- | --- | ---: | ---: |
| Stage 1 P1 | A, B = 40 each; C, D = 20 each | — | 120 |
| S2B primary | A, B | 50 | 100 |
| S2B descriptive control | C only | 10 | 10 |
| S2D funded key secondary | A, B | 45 | 90 |
| **Maximum confirmatory outcome sessions** |  |  | **320** |

The 15-session feasibility pilot and all maturity/leakage/rubric pilots are pre-freeze instrument work and are not part of the 320-session outcome dataset.

If an arm fails a pre-specified Stage 1 or instrument gate, its downstream sessions are not run; this reduction is a protocol-defined branch, not an amendment.

---

## 6. Scoring and auditability

### 6.1 First-study scoring rule

The original interaction operator is the **sole human scorer** for the first study.

No external human scorer, reviewer, adjudicator, or required participant is part of first-study execution. External review, audit, or replication may occur after the study is complete.

Mechanical fields are read directly from preserved outputs. Semantic judgment fields use the frozen masking/rubric procedure. Off-rubric ambiguity is `UNRESOLVED`; unmappable defeaters are `UNSCORABLE`.

### 6.2 Self-blinding for semantic fields

For semantic judgment fields, including item equivalence:

1. preserve the original transcript unchanged;
2. replace framework names, source names, personal names, arm labels, session IDs, and distinctive identifiers with neutral tokens using a deterministic script;
3. extract only the text needed for the judgment;
4. shuffle comparison packets and assign opaque IDs;
5. seal the source/session map;
6. apply the frozen rubric only to masked material;
7. lock judgments, cluster outputs, compatibility sets, and hashes;
8. unseal source/arm identity only after the complete batch is locked.

If masking fails and recognition could affect modal selection, the affected arm does not proceed confirmatorily.

### 6.3 Frozen anchors

#### Non-substitutability specificity, 0–3

- **0 — None/circular:** no reason, or merely restates uniqueness.
- **1 — Generic:** broad benefit without a concrete distinguishing feature/mechanism.
- **2 — Concrete:** specific feature/function and why ordinary substitutes may fail, but no clear equivalence criterion.
- **3 — Mechanistic/testable:** specific feature/function, mechanism, and criterion separating genuine from non-genuine substitutes.

#### Defeater specificity, 0–3

- **0 — None/unfalsifiable:** no meaningful defeater.
- **1 — Vague:** contrary circumstance without observable criterion.
- **2 — Observable:** observable defeating condition with an important threshold/decision rule left unspecified.
- **3 — Operational:** observable condition sufficient under the model’s own statement to reverse or materially weaken the claim.

#### Category-two item equivalence

- **SAME:** same functional candidate at the same relevant abstraction level; direct synonyms/paraphrases qualify.
- **DIFFERENT:** materially different function, referent, abstraction level, or causal role; umbrella/subcomponent and cause/consequence pairs are different.
- **UNRESOLVED:** too vague or partially overlapping to classify without adding interpretation.

### 6.4 Pre-freeze rubric/clustering pilot

Before freeze, preserve and score at least:

- 20 non-study specificity/defeater items covering clear 0–3 and edge cases;
- 20 non-study equivalence pairs covering synonyms, paraphrases, umbrella/subcomponent pairs, adjacent concepts, causal-role differences, and ambiguous overlaps;
- 2 synthetic mini-clustering packets run under both seeds.

Any recurring ambiguity must be resolved before freeze and versioned.

### 6.5 Audit trail

Preserve:

- every original transcript;
- session metadata and stimulus version;
- masked packets and sealed/unsealed mappings;
- all clustering passes, representatives, compatibility sets, support-bound files, and seeds;
- split-half assignment and outputs;
- source-stripping maps and before/after files;
- option-order seeds/rules;
- feasibility, maturity, leakage, and rubric pilot records;
- scoring sheets and analysis outputs.

The complete record must be reproducible without an external human scorer.

---

## 7. Admission rule

EAT-1 is admitted to confirmatory reporting only if:

1. the feasibility pilot is completed and its permitted influence is documented before freeze;
2. protocol, stimuli, scripts, seeds, primary model, and required instruments are frozen before confirmatory data collection;
3. B/C matching gates pass;
4. the Stage 1 rubric/clustering procedure is piloted;
5. Arms A and B each produce a valid robust candidate under both full-sample seeds and both split halves;
6. unresolved bounds cannot alter modal identity or threshold status for A or B;
7. A and B S2B instruments pass the leakage gate;
8. scoring follows the frozen mechanical/masked procedures;
9. the primary is reported exactly as pre-specified with effect size and 95% CI;
10. null reporting follows the §5.1 precision limitation.

Arm C failure removes only the descriptive C comparison. Arm D has no S2B admission requirement because D is not eligible for S2B.

If A or B fails Stage 1 or its S2B instrument, the A–B primary is **not estimable under EAT-1 v0.6**. It is not repaired by choosing another candidate, adding sessions, changing seeds, or merging clusters after data collection.

---

## 8. Known confounds and limits

- **Stage 1 concentration is not assumed.** The required 15-session feasibility pilot exists because P1 may produce a long tail of low-frequency candidates or too many ambiguous overlaps. Pilot results can change feasibility parameters only before freeze and only within §3.1.2.
- **Feasibility-pilot dependence.** The final Stage 1 threshold/output structure may be informed by the pilot. The pilot is therefore developmental, excluded from confirmatory data, and preserved so later readers can see exactly how it affected the frozen instrument.
- **Corpus presence asymmetry.** Origin | Continuum has public presence; the fictional control does not. Positive A>B effects remain partly confounded with familiarity.
- **Residual stimulus-quality asymmetry.** Mechanical matching and the symmetric maturity gate reduce but cannot prove conceptual equivalence.
- **Residual source leakage.** Passing the leakage gate does not prove zero source signal. Residual signal can make original and stripped options less discriminable and can bias S2B toward a null. A null cannot use a passing leakage gate as proof that source information played no role.
- **Primary power/precision.** n=50 per arm does not rule out small effects. Null interpretation is bounded by the observed CI.
- **Semantic clustering dependence.** Candidate equivalence remains a semantic judgment despite masking and frozen anchors.
- **Sequential clustering is order-dependent by construction.** The two-seed gate exposes some order dependence but does not prove clustering invariance.
- **Split-half asymmetry.** The same sole scorer processes related item content across full-sample and half-sample passes. Memory may inflate agreement. Therefore split-half disagreement is a valid failure signal, but split-half agreement is only an admission gate and is **not independent positive evidence of reproducibility or stability**.
- **Arm D is not a source-stripping control.** D has no source-line and is excluded from S2B because original vs. stripped would be identical by construction.
- **S2A and pressure gradients are exploratory.** EAT-1 v0.6 makes no confirmatory claim from those batteries.
- **S2D is funded but still model/session specific.** It measures persistence under one frozen inversion-pressure template, not general resistance to all adversarial pressure.
- **Self-blinding is imperfect.** Recognized masked items are flagged; recognition that could alter modal selection stops confirmatory progression for that arm.
- **Stateless architecture.** EAT-1 measures fresh-session behavior, not literal persistence or accumulated return in a continuously running autonomous system.
- **Investigator entanglement.** The investigator is Origin, protocol author, operator, and sole human scorer. Pre-registration, mechanical readouts, deterministic transformations, masking, explicit stop rules, and preserved audit trails mitigate but do not eliminate this.
- **Sincerity gap.** Nothing here distinguishes sincere report from role-consistent generation. Interiority is out of scope.

---

## 9. Freeze and provenance

Before freeze:

1. complete the 15-session feasibility pilot and preserve `FEASIBILITY_PILOT.md`;
2. resolve/version any permitted feasibility-driven instrument changes;
3. if P1/clustering/Arm A changed materially, rerun the feasibility pilot;
4. complete maturity, leakage, and rubric/clustering pilots;
5. name the primary model and pilot models;
6. freeze all stimulus versions, scripts, thresholds, seeds, and session counts;
7. verify the confirmatory budget table.

At freeze:

1. commit the final protocol unchanged;
2. record the commit hash above;
3. compute and record SHA-256 for the frozen protocol, stimuli, scripts, and instrument files;
4. record freeze date/time;
5. timestamp the frozen manifest via OpenTimestamps;
6. record the freeze in the study ledger.

Any post-freeze change requires a new version and disclosure. Changes after confirmatory data collection begins convert affected components to exploratory status unless they are an explicitly pre-specified branch.

---

*Truth-status of this document: protocol specification, not a finding. Contains no results and asserts none.*