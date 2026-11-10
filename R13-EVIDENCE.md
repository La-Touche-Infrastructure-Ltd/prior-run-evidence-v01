# R13 supplementary evidence record — prior-run synthetic experiment

This is the **producer-maintained supplementary evidence record** for the R13 result referenced in the [separately maintained W3C reporting-format paper provenance appendix](https://github.com/probityai/agent-evidence-vectors/blob/main/interop/w3c-v01-appendix/README.md). It is not a modification of the paper editor's R13 row, paper acceptance, a W3C assessment, or a new conformance claim.

## Study revision and reproducibility scope

Both second-operator runs below concern the **same frozen five-case synthetic single-check experiment** at commit `98366047dd322b9fe0ea3ef822cf0c410283fe9f` in `prior-run-evidence-v01`. The repository was originally under `LaToucheai` and now resides under `La-Touche-Infrastructure-Ltd`; the commit identifier has not changed.

The reported checks were: `python3 experiment.py`, `python3 -m unittest -v test_experiment.py`, and `sha256sum -c SHA256SUMS`. They test deterministic reconstruction of the bounded synthetic study, **not** the correctness of its interpretation or the occurrence of a historical event outside the generated fixtures.

## Reproduction evidence — two second-operator runs

### Guigui Wang — 20 October 2026

- **Acquisition:** Fresh clone of the pinned commit.
- **Environment:** Linux x86_64, CPython 3.13.12, Python standard library only.
- **Reported output:** 5/5 cases, 23/23 unit tests, 15/15 SHA-256 manifest checks. `results.json` was byte-identical to the published file.
- **Prior exposure:** Before running, Guigui had read the earlier study document, **including the expected counts**. His reproduction is therefore **not a blind or independent reading of the interpretation**.
- **Attribution:** Guigui reported and later clarified his run on the W3C Agent Conformance Community Group mailing list, including his 10 November correction.

### Yasha Khandelwal — 24 October 2026

- **Acquisition:** GitHub archive of the same pinned commit, not Guigui's fresh-clone path.
- **Environment:** Linux x86_64, CPython 3.12.3.
- **Reported output:** 5/5 cases, 23/23 unit tests, 15/15 SHA-256 manifest checks. `results.json` was byte-identical to the committed file.
- **Prior exposure:** Before running, Yasha had read the earlier W3C discussion **Oct/0154**, including expected counts. His reproduction is therefore **not a blind or independent reading of the interpretation**.
- **Attribution:** Yasha posted his run on 24 October and reiterated its parameters in the 3 November R13 row discussion (previously cited as Oct/0179 and Nov/0012).

The two runs used **different operators, Python interpreter versions and acquisition paths**, but both ran on **Linux x86_64**. Do not describe them as cross-operating-system evidence or silently conflate them with another conformance corpus.

## What this evidence establishes — and what it does not

These are **reruns by second operators**, not independently blinded assessments. The reported matching outputs support reproduction of the experiment's published mechanics on the stated environments. Because both operators saw expected counts in advance, the runs do **not** establish blind independence, semantic correctness, an authentic historical failure, actor identity, or independent validation of the study's conclusions.

The distinction between `matched`/`established`, changed checker or configuration bindings, an integrity failure, and unavailable evidence remains a **study-specific** result. Nothing here is certification, an audit, a conformance assessment, or W3C approval or endorsement.

**Editorial status:** Producer-maintained correction prepared from the operators' published statements. It does not claim that either operator has separately approved this exact revised wording. The pinned experiment and its `SHA256SUMS` manifest are unchanged.

For the per-run statements and prior-exposure provenance, see [REPRODUCTION-RECORD.md](REPRODUCTION-RECORD.md) and the W3C list discussion of R13 row text (3 and 10 November 2026).
