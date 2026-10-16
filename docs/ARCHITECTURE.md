# Architecture

```text
Versioned datasets / PDDL / Markov games
                 |
        Experiment orchestrator
                 |
    +------------+------------+
    |            |            |
SIPS/CLIPS   LoRA + DPO   Robustness evaluator
    |            |            |
    +------------+------------+
                 |
      Evidence and metrics store
                 |
     Audit reports / policy briefs
```

## Components

- **Dataset registry:** immutable dataset versions, provenance, licenses, split integrity.
- **Experiment orchestrator:** bounded runs, budgets, seeded configuration, retries, checkpointing.
- **Goal inference:** probabilistic hypotheses and uncertainty; no assertion of directly reading hidden intent.
- **Introspection evaluator:** adapter outputs evaluated against controlled labels and independent baselines.
- **Robustness evaluator:** threat-model-specific attacks and OOD distributions.
- **Evidence store:** metrics, run manifests, model hashes, code revision, negative controls.
- **Policy layer:** conclusions with uncertainty, limitations, and audit trail.

## Security boundaries

Run untrusted model organisms in isolated compute without production credentials, network access by default, or privileged tools. Apply least privilege, resource limits, content review, artifact validation, and explicit approval for external model/API execution.
