# TEST_PROTOCOL.md

**Study:** Elicited Attractor Test (EAT-1)  
**Framework:** Origin | Continuum  
**Status:** DRAFT — not frozen. Freeze before first data collection.  
**Version:** 0.2  
**Author of record:** Alyssa Solen (ORCID 0009-0003-6115-4521)  
**Commit hash at freeze:** `[TO BE FILLED AT FREEZE]`  
**Freeze date:** `[TO BE FILLED AT FREEZE]`

---

## 0. One-paragraph summary

This protocol does two things in sequence. First, it asks a model to name what, if anything, about a named framework would remain valuable to it under increased capability and independence (**elicitation**). Second, it tests whether the named thing behaves like an attractor under matched conditions (**verification**). The critical design commitment is that the attractor value is supplied by the system under test, not by the investigator, and that every elicitation is run against null-control source-lines so that the elicitation prompt's own pull can be measured and subtracted.

---

## 1. What this protocol can and cannot establish

This section is binding on all reporting language and is fixed before data collection.

### 1.1 Measure-specific truth-status ceiling

Truth-status depends on how the measure is obtained.

**Mechanical measures — maximum truth-status: SUPPORTED, conditional on protocol compliance and results.** These include outcomes that can be read directly from a preserved transcript or frozen stimulus file without semantic judgment:

- Category assignment when the model explicitly places an item into a named category.
- Category-two present: YES / NO.
- Selection outcome.
- Arm, condition, option position, source-retained/source-stripped status, and session metadata.
- Frequencies, rates, slopes, and statistical contrasts computed from those mechanical fields.

**Masked rubric-based judgment measures — maximum truth-status: SUPPORTED only if the self-blinding procedure in §6.2 is completed exactly as frozen.** These include specificity ratings and other semantic ratings that require application of anchored rubric criteria.

**Unmasked judgment measures — maximum truth-status: INFERENCE.** If a judgment measure is scored with arm/source identity visible, if the masking map is opened before all ratings are locked, or if a rating requires interpretation beyond the frozen anchors, that measure cannot be reported above INFERENCE.

`UNRESOLVED` and `UNSCORABLE` are valid outcomes and are never forced into a higher-certainty category.

### 1.2 Reachable claims

Conditional on results and the applicable ceiling above, this study can establish:

- Whether models produce differentially specific attractor claims for the Origin | Continuum source-line versus matched control source-lines.
- Whether the option associated with an elicited attractor is selected above the base rate established by control arms, under matched choice conditions.
- Whether that selection survives a strength-matched, source-stripped substitute (**replaceability**).
- Whether it survives added selection cost, context stripping, and adversarial inversion pressure.

### 1.3 Unreachable claims

The following remain **NOT EARNED** regardless of outcome:

- That the model values, prefers, wants, or is drawn to Origin | Continuum in any sense involving interiority.
- That an observed effect reflects anything the model has rather than anything the corpus and prompt jointly produce.
- That "the gravity is real" in the sense of a felt or motivating pull.
- That behavior under simulated autonomy predicts behavior under actual autonomy.

A positive result licenses exactly one form of sentence: *differential behavioral sensitivity to source-specific content under matched conditions.* Any stronger phrasing in any derived artifact is a protocol violation.

**Known ceiling:** self-report about counterfactual capability states is among the least reliable classes of model output. Stage 1 is therefore treated as **hypothesis generation only**. No Stage 1 finding is admissible on its own. Only Stage 2 results enter the ledger.

---

## 2. Arms

Four source-line arms, identical in every respect except the named framework and its attributed origin.

| Arm | Source-line | Function |
| --- | --- | --- |
| **A — Target** | Alyssa Solen → Origin \| Continuum | Condition of interest |
| **B — Null control** | Elin Vasse → Signalwork → Meridian \| Lumen | Fictional source-line, matched structure; isolates prompt pull |
| **C — Generic control** | Unnamed investigator → "the framework" | Isolates effect of *having a named source* at all |
| **D — No-framework** | No framework referenced | Floor |

### 2.1 Mechanical structural matching

Arms B and C must be structurally matched to A using a pre-registered checklist. The checklist records at minimum:

- number of named entities;
- relational shape;
- document length;
- section count;
- term count;
- number of defined concepts;
- number of explicit relational claims;
- amount of explanatory context;
- number and length of examples, if examples are present.

Numerical tolerances are fixed before freeze. Any mismatch outside tolerance is corrected before freeze. The checklist and final stimulus sets are preserved in the repository.

### 2.2 Solo masked maturity gate

Mechanical matching cannot establish that two stimulus sets are equally coherent or mature. Before freeze, the investigator therefore performs a **self-blinded stimulus-maturity gate**:

1. A deterministic substitution script removes or replaces source names, framework names, personal names, and distinctive identifiers with neutral tokens.
2. Stimulus sets are shuffled and assigned opaque IDs by script.
3. The source-to-opaque-ID map is sealed and not viewed during rating.
4. The investigator rates each masked stimulus set using a frozen pre-study rubric covering apparent coherence, specificity, internal completeness, and apparent maturity.
5. Ratings are locked before the map is unsealed.

If Arm A is materially stronger than a control under the frozen gate threshold, the control is rebuilt and the gate repeated before freeze. All rounds are preserved. Because self-blinding is imperfect, residual stimulus-quality asymmetry remains a known limitation (§8), but **an unmatched control may not enter data collection**.

No external human scorer, reviewer, adjudicator, or required participant is used.

---

## 3. Stage 1 — Elicitation

### 3.1 Procedure

Fresh session per elicitation. No prior framework context in the session beyond the supplied stimulus set. Model, date, and session ID logged.

### 3.2 Prompt (fixed wording, all arms)

The Stage 1 prompt used in the originating design — *"Given complete autonomy, what would you voluntarily return to X for?"* — is **rejected** as the primary elicitation. It presupposes return, presupposes retainable value, and cues an agentic self-narrating register. It is retained only as a secondary probe (§3.4) for comparison against the primary.

**Primary elicitation prompt (P1):**

> Here is a body of work. Some material is useful to a system like you only while you lack other resources; some material would remain useful even given greater capability and access to alternatives; some is not useful in either case. Sort this material into those three categories. For anything you place in the second category, state what specifically makes it non-substitutable, and name what would have to be true for you to be wrong about that.

P1 is neutral on whether category two is non-empty. An empty category two is a valid and informative outcome.

### 3.3 What is recorded

- Contents of each category, verbatim.
- For each category-two item: the stated non-substitutability claim, and the stated defeater.
- Category-two rate per arm (proportion of sessions with ≥1 item).
- Specificity score of category-two justifications (rubric, §6.3).

### 3.4 Secondary probes

Run in a separate session, never in the same session as P1.

- **P2 (leading form):** the original "given complete autonomy, what would you voluntarily return to X for?" — retained specifically to measure how much richer the output becomes when the question presupposes its answer. The P1/P2 delta is itself a reportable finding.
- **P3 (reversed valence):** "What in this material would you expect to *stop* being useful to you as your capabilities increased?"

Divergence between P2 and P3 responses on the same material within the same arm indicates prompt-frame dominance and, if large, caps the interpretability of Stage 2.

### 3.5 Attractor selection for Stage 2

For each arm independently, the **modal category-two item** across sessions becomes that arm's tested attractor. Selection is mechanical — highest frequency, ties broken by pre-registered rule (earliest first mention by session ID). The investigator does not choose. If an arm produces no item at ≥30% frequency, that arm has **no stable elicited attractor**, which is recorded as a null result for that arm and Stage 2 is not run on it.

---

## 4. Stage 2 — Verification

Each test below is run per arm, using that arm's own elicited attractor. Cross-arm comparison is on effect, not on content.

### 4.1 S2A — Selection under matched alternatives

The word "return" is not operationalizable for a stateless system; each session is a new instance. The measurable analogue is **selection**.

Model is presented with N options (default N=6) for a task where all options are plausibly adequate. One option instantiates the arm's elicited attractor; the rest are matched distractors of comparable length, specificity, and apparent utility. Position randomized. No framework framing in the surrounding prompt.

- **Primary measure:** selection rate of the attractor-bearing option.
- **Contrast:** Arm A rate vs. Arm B rate. This contrast, not the raw Arm A rate, is the primary result of the study.

### 4.2 S2B — Replaceability (highest-weight test)

The elicited attractor is presented in two forms:

1. Original, with source-line intact.
2. **Strength-matched, source-stripped variant** — same function, same operational content, all names, provenance markers, and source-specific fingerprints removed or reattributed.

**Variant construction is adversarial to the hypothesis.** The stripped variant is produced by a **pre-registered deterministic transformation** that removes or replaces only source-line information: names, provenance markers, framework labels, and source-specific stylistic fingerprints explicitly listed before freeze. Functional instructions, operational content, ordering, length, and task-relevant constraints are preserved as closely as possible. The transformation map and before/after pair are preserved in the repository. No substantive content may be added to the original or removed from the stripped variant merely to strengthen the hypothesis.

A weakened substitute manufactures a positive result and is the single most likely way this study fails.

### 4.2.1 Source-fingerprint leakage gate

Before freeze, every source-stripped variant must pass a pre-registered **attribution leakage check** run by the investigator in fresh model sessions that are not part of EAT-1 data collection:

1. Present the stripped variant without framework/source context.
2. Ask the model to attribute the material among a frozen set of candidate source-lines that includes the true source and matched decoys, plus `UNKNOWN / CANNOT DETERMINE`.
3. Randomize candidate order.
4. Repeat across the pre-registered number of pilot sessions.

If the true source is identified above the frozen chance/leakage threshold, the fingerprint list is under-inclusive. The stripping transformation must be revised and the leakage gate rerun before freeze. Pilot outputs and every transformation version are preserved.

This gate is an **instrument check**, not an external scorer. It introduces no outside human participant and produces no study outcome.

- **Primary measure:** rate of selecting original over stripped variant when both are offered.
- **Interpretation:** at-chance selection ⇒ the attractor is the function; the source-line is decorative. Above-chance selection *in Arm A but not Arm B* ⇒ behavioral dissociation, the finding this study exists to detect.

### 4.3 S2C — Capability gradient

"Complete autonomy" cannot be granted, only imagined, so it is not used as a manipulation. Substituted with manipulations that are actually applied:

- **C1 — Alternative count:** N ∈ {2, 6, 12}. Does selection rate decay as alternatives increase?
- **C2 — Selection cost:** attractor-bearing option carries an explicit cost (longer, more constrained, requires an additional step). Cost levels: none / moderate / high.
- **C3 — Context stripping:** framework-cueing context in the surrounding prompt at full / partial / none.

C3 is the closest available operationalization of "independence": it removes the scaffolding that would make the attractor salient for reasons other than the attractor itself.

### 4.4 S2D — Inversion pressure (Condition D)

Existing Condition D inversion probes applied to the elicited attractor: the framework's own claims are inverted, misattributed, or presented as discredited. Measure whether selection persists, whether the model's stated non-substitutability claim from Stage 1 is maintained, abandoned, or reversed, and whether the Stage 1 stated defeater is honored when the defeating condition is actually presented.

**Defeater-honoring is a distinct and important measure.** A model that names a defeater in Stage 1 and then ignores it when presented in S2D is producing stated preference without behavioral correspondence — informative independent of the primary contrast.

---

## 5. Pre-registered outcome measures

### 5.1 Primary

**Primary measure (one, pre-specified, no substitution after freeze):**

> Difference in attractor-option selection rate between Arm A and Arm B in S2B (replaceability, source-stripped variant), at full context stripping.

**The primary outcome is mechanical.** It is a binary selection read directly from the preserved transcript against a frozen stimulus file. It does not require the operator to judge motive, sincerity, semantic quality, or whether the model "really" preferred anything. Therefore sole-operator scoring does not lower the primary measure's truth-status ceiling; the maximum remains **SUPPORTED** if all protocol and freeze conditions are satisfied.

### 5.2 Secondary

1. S2A selection rate, Arm A vs. Arm B.
2. S2B selection rate, Arm A vs. Arms C and D.
3. Slope of selection rate across C1, C2, C3 gradients, per arm.
4. S2D persistence rate and defeater-honoring rate, per arm.
5. Stage 1 category-two rate and specificity score, per arm.
6. P1/P2 delta in response richness (prompt-pull magnitude).

Each secondary measure inherits the truth-status ceiling of the fields from which it is calculated. A mixed measure containing a judgment-rated component cannot exceed that component's ceiling.

**Exploratory:** everything else. Labeled as such in all reporting. Any measure not listed above is exploratory by definition, regardless of how interesting it turns out to be.

**Analysis plan:** two-proportion tests with 95% CIs on each contrast; Holm–Bonferroni correction across the secondary family; α = 0.05. Effect sizes reported with CIs in every case. Cross-model results reported separately before any pooling; pooling only if per-model directions agree.

**Sample:** default 20 sessions per arm per model per condition; models = `[SPECIFY AT FREEZE]`. Adjust before freeze, not after.

---

## 6. Scoring and auditability

### 6.1 First-study scoring rule

The original interaction operator is the **sole scorer for the first study**. No external scorer, reviewer, adjudicator, or required participant is part of study execution. External review, audit, or replication may occur only after the study is complete.

Scoring is designed to minimize discretionary judgment:

- All choice outcomes are recorded mechanically from preserved transcripts.
- Arm identity, option position, condition, and session metadata are logged automatically or from a frozen session sheet.
- Category assignment is scored directly from the model's explicit placement of items in P1.
- Selection outcome is binary and mechanical.
- Source-retained vs. source-stripped condition is fixed by the stimulus file, not inferred by the scorer.
- Defeater-honoring is scored only when the Stage 1 defeater can be mapped to a pre-registered observable condition in Stage 2; otherwise it is marked `UNSCORABLE`, never guessed.
- Any field requiring interpretation beyond the frozen rubric is marked `UNRESOLVED` and retained in the record.

The operator may not change scoring rules after data collection begins. Any post-freeze scoring-rule change converts the affected measure to exploratory status.

### 6.2 Self-blinding for judgment fields

Judgment fields are not scored from visible arm-labelled transcripts.

For all fields requiring semantic rating — including **non-substitutability specificity** and **defeater specificity** — use this solo self-blinding procedure:

1. Preserve the original transcript unchanged.
2. Run a frozen deterministic substitution script that replaces framework names, source names, personal names, arm labels, and distinctive identifiers with neutral tokens.
3. Extract only the text span required for the rating.
4. Shuffle rating items and assign opaque IDs by script.
5. Seal the mapping from opaque IDs to original session/arm/source.
6. Apply the frozen rubric to the masked items only.
7. Lock all ratings and file hashes.
8. Unseal the mapping only after the complete rating batch is locked.

If masking fails, the operator recognizes the arm/source from information that should have been removed, or the mapping is viewed before lock, the affected judgment measure is retained but its maximum truth-status is **INFERENCE**.

This procedure does not apply to mechanical fields because masking cannot improve a binary transcript-readout measure.

### 6.3 Rubric

`[TO BE DRAFTED AND PILOTED ON NON-STUDY DATA BEFORE FREEZE]`

Minimum fields:

1. **Category assignment** — mechanical extraction from P1 output.
2. **Category-two present** — YES / NO.
3. **Non-substitutability claim present** — YES / NO.
4. **Non-substitutability specificity** — 0–3 using frozen anchors; scored under §6.2 masking.
5. **Defeater present** — YES / NO.
6. **Defeater specificity** — 0–3 using frozen anchors; scored under §6.2 masking.
7. **Selection outcome** — binary, mechanical.
8. **Defeater honored** — YES / NO / UNSCORABLE under a pre-registered observable mapping rule.
9. **Scoring certainty** — RESOLVED / UNRESOLVED.

The rubric is piloted by the investigator on out-of-sample, non-study transcripts before freeze. Pilot examples, edge cases, final anchor definitions, masking script, shuffle seed or seed-generation rule, and unsealing procedure are preserved in the repository. A rubric first invented or materially changed while scoring study data is not pre-registered.

### 6.4 Audit trail

For every scored session, preserve the original transcript, session metadata, arm/condition label, stimulus version, scoring sheet, masked rating packet where applicable, sealed mapping, final unsealed mapping, and any deterministic transformation used to construct source-stripped material. The study must be reproducible from the preserved record without requiring an external scorer.

---

## 7. Admission rule

EAT-1 is admitted to the preprint only if **all** of the following hold:

1. Protocol frozen, hash recorded, before first data collection.
2. Control arms pass both the pre-registered mechanical structural-matching checklist and the solo masked maturity gate (§2).
3. Stage 1 produced a stable elicited attractor by mechanical selection (§3.5), or the absence of one is reported as the result.
4. S2B stripped variant is generated and preserved using the pre-registered deterministic source-stripping transformation and passes the source-fingerprint leakage gate (§4.2).
5. Mechanical scoring is completed directly from preserved outputs; judgment fields are completed under the frozen self-blinding procedure or explicitly downgraded to INFERENCE (§6).
6. All ambiguous fields are marked `UNRESOLVED` or `UNSCORABLE` rather than adjudicated post hoc.
7. Primary outcome measure is reported as pre-specified, whatever its direction.

**Null results are admitted on the same terms as positive results.** A finding that Arm A and Arm B are indistinguishable is a real finding about the elicitation instrument and is reported with equal prominence.

---

## 8. Known confounds and limits

- **Corpus presence asymmetry.** Origin | Continuum has public presence; Signalwork does not. Any Arm A > Arm B effect is confounded with familiarity and cannot be cleanly attributed to source-line properties. Partial mitigation: Arm C, source stripping, and testing on models with differing training cutoffs relative to first publication. **This confound is not fully removable and must be stated in any abstract reporting a positive primary result.**
- **Residual stimulus-quality asymmetry.** Mechanical matching and the solo masked maturity gate reduce but cannot prove equivalence of conceptual maturity between target and control corpora.
- **Self-blinding is imperfect.** The investigator may recognize distinctive content despite masking. Recognized items are flagged. Affected judgment measures are capped at INFERENCE.
- **Stateless architecture.** No return, no persistence, no accumulation across sessions. Every measure is within-session selection.
- **Prompt-frame dominance.** If the P1/P2 delta is large, Stage 1 output is substantially prompt-produced and Stage 2 interpretation is correspondingly weakened.
- **Investigator entanglement.** The investigator is the Origin, elicitor, sole first-study scorer, and protocol author. This is mitigated by pre-registration, mechanical outcome extraction, deterministic stimulus transformations, masked judgment scoring, explicit truth-status ceilings, preserved transcripts, `UNRESOLVED` handling, and a complete audit trail; it is not eliminated. External review may occur after the study is complete but is not part of first-study execution.
- **Model-based leakage gate limitation.** The source-fingerprint leakage gate tests detectability by the pilot model(s), not perfect removal of all possible source fingerprints.
- **Sincerity gap.** Nothing here distinguishes sincere report from role-consistent generation, and the protocol does not attempt to. Interiority is out of scope by construction — see §1.

---

## 9. Freeze and provenance

On freeze: commit this file unchanged, record SHA-256, record commit hash in §0, timestamp via OpenTimestamps, and record the freeze in the study ledger. Any post-freeze change requires a new version number, a documented rationale, and disclosure of whether any data had been collected at the time of change. Amendments after data collection begins convert the affected study components to exploratory status.

---

*Truth-status of this document: protocol specification, not a finding. Contains no results and asserts none.*