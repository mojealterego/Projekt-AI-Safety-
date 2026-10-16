# Research protocol

## Hypotheses

H1: Behavioral goal inference improves detection over prompt-only baselines on controlled sandbagging tasks.

H2: Introspection adapters improve recall without unacceptable false positives on held-out model organisms.

H3: Distribution-shift evaluation exposes failure modes missed by in-distribution tests.

These are **hypotheses**, not established results.

## Evaluation

Pre-register dataset splits, baselines, confidence intervals, and primary endpoints before training. Measure AUROC, AUPRC, false-positive rate at fixed recall, verbalization rate, calibration, and OOD degradation. Record seed variance and ablations. Prevent train/test leakage and benchmark contamination.

## Reporting

Every result must include code commit, model and dataset identifiers, compute configuration, costs, reproducibility instructions, and limitations. Claims about intent require corroborating behavioral evidence; model self-reports alone are not ground truth.

## Source

Primary project specification: *Wniosek Grantowy AI Safety Singapore* (user-provided PDF, 11 pages). Program and external research claims require independent verification.
