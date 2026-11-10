# Second-operator reproduction record — Guigui Wang and Yasha Khandelwal

Supplementary **producer-maintained** reproduction evidence for the five-case synthetic single-check prior-run experiment. This record does not modify the pinned commit or any file listed in its `SHA256SUMS` manifest.

**Pinned revision:** `98366047dd322b9fe0ea3ef822cf0c410283fe9f`, originally published under `LaToucheai/prior-run-evidence-v01`, now `La-Touche-Infrastructure-Ltd/prior-run-evidence-v01`.

## Reproduction 1 — Guigui Wang, 20 October 2026

Guigui Wang (Correctover — AI Reliability) **reran the experiment as a second operator** from a **fresh clone** of the pinned revision.

- **Platform:** Linux x86_64.
- **Interpreter:** CPython 3.13.12, standard library only.
- **Checks reported:** 5/5 cases, 23/23 unit tests, 15/15 SHA-256 manifest hashes.
- **Output:** `results.json` byte-identical to the published file.
- **Prior exposure:** Guigui had read the earlier study document and its **expected counts before running**. This was **not a blind, interpretation-independent evaluation**.

Guigui confirmed the parameters on the W3C mailing list on 3 November and again on 10 November 2026; his 10 November correction asked specifically that prior exposure appear in the record, and that the phrase “independently reran” be replaced.

## Reproduction 2 — Yasha Khandelwal, 24 October 2026

Yasha Khandelwal separately **reran the same pinned revision as a second operator**, obtaining it from the **GitHub archive**, rather than by Guigui's fresh-clone route.

- **Platform:** Linux x86_64.
- **Interpreter:** CPython 3.12.3.
- **Checks reported:** 5/5 cases, 23/23 unit tests, 15/15 SHA-256 manifest hashes.
- **Output:** `results.json` byte-identical to the committed file.
- **Prior exposure:** Yasha had read the earlier W3C **Oct/0154** material, **including expected counts before running**. This was **not a blind, interpretation-independent evaluation**.

Yasha recorded the run on 24 October and restated the acquisition method, environment and outcome in the 3 November R13 discussion (earlier references Oct/0179 and Nov/0012). Guigui acknowledged the separate Yasha run in his 10 November correction.

## Reproduction commands and limits

The published experiment uses:

```sh
python3 experiment.py
python3 -m unittest -v test_experiment.py
sha256sum -c SHA256SUMS
```

Both reported runs reached the same expected counts with byte-identical output across **two interpreter versions and two acquisition paths on Linux**. This establishes reported reproducibility of **bounded synthetic mechanics** under the stated conditions, not blind independence, the correctness of the study's interpretation, authentication of the actor who generated a historical record, or proof that a real-world historical failure happened.

Neither run is a W3C assessment, a conformance certification, an audit, or endorsement of the study's broader claims. A different operator running producer-authored code is not the same as an independent implementation or a blind assessment.

**Editorial/provenance note:** This updated text is maintained by the study producer, based on the operators' published statements. It is **not presented as either operator's verbatim report or their approval of this particular wording**. The frozen commit and experimental results remain unchanged.

See [R13-EVIDENCE.md](R13-EVIDENCE.md) for the associated bounded-claim record.
