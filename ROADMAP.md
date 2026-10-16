# Research roadmap

Status key: [ ] planned; [x] verified complete.

## Phase 0 — Research foundations
- [x] Create repository documentation and research roadmap.
- [ ] Verify grant-program dates, eligibility, budget terms, and research references against primary sources.
- [ ] Define research questions, baselines, hypotheses, and acceptance thresholds.
- [ ] Establish dataset governance, licenses, model permissions, and experiment ethics.
- [ ] Implement CI, static analysis, dependency pinning, and reproducible environments.

## Phase 1 — Weeks 1–3: normative environments and model organisms
- [ ] Implement PDDL scenarios and Markov-game environments.
- [ ] Create a versioned AuditBench schema with train/test/OOD separation.
- [ ] Generate controlled model organisms for sandbagging and concealed behaviors in isolated research settings.
- [ ] Implement baseline goal-inference methods and SIPS/CLIPS prototypes.
- [ ] Validate labels, controls, and data provenance.

## Phase 2 — Weeks 4–7: introspection
- [ ] Implement LoRA adapter training and evaluation.
- [ ] Add DPO refinement and matched negative controls.
- [ ] Integrate CLIPS evidence with independent behavioral observations.
- [ ] Measure calibration, false-positive rate, and generalization.

## Phase 3 — Weeks 8–10: robustness
- [ ] Implement distribution-shift threat models for discrete text.
- [ ] Evaluate ADT-style training and suitable text-domain perturbations.
- [ ] Assess applicability of EasyRobust, PGD, AutoAttack, MM-LDA, and RCE; do not assume vision attacks transfer unchanged to text.
- [ ] Report AUROC, verbalization rate, false-positive rate, confidence intervals, and OOD results.
- [ ] Add Gumbel-Softmax or gradient-free fallback where justified.

## Phase 4 — Weeks 11–12: synthesis and governance
- [ ] Publish reproducible benchmarks and documented limitations.
- [ ] Produce research paper and policy brief drafts.
- [ ] Complete independent review, security assessment, and release checklist.

## Continuous quality gates
- [ ] Provenance and reproducibility of every result.
- [ ] Separate observed behaviors from inferred intent.
- [ ] No claim that adapter reports reveal ground truth without independent validation.
- [ ] No production-readiness claim without integration and security evidence.
