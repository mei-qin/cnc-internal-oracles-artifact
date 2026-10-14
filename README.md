# Auditable Internal Test Oracles for CNC Software

Research artifact for **Constructing Auditable Internal Test Oracles for Multi-Stage CNC Control Software** (S5-M R3, refocused manuscript).

This repository provides a fixed public inspection edition of the existing CNC oracle evidence. It includes frozen observations, checker/reference implementations, protocols, amendments, source-adjudication records, and paper-to-evidence indexes. It is a research artifact, not a production CNC release.

## Download the fixed artifact

Use release **s5-m-r3-refocused-v1.0.0**:

- [Release and download files](https://github.com/mei-qin/cnc-internal-oracles-artifact/releases/tag/s5-m-r3-refocused-v1.0.0)
- [Artifact ZIP](https://github.com/mei-qin/cnc-internal-oracles-artifact/releases/download/s5-m-r3-refocused-v1.0.0/CNC_INTERNAL_ORACLES_ARTIFACT_v1.0.0.zip)
- [SHA-256 checksums](https://github.com/mei-qin/cnc-internal-oracles-artifact/releases/download/s5-m-r3-refocused-v1.0.0/SHA256SUMS.txt)

The ZIP is a release asset, separate from GitHub's automatically generated source-code ZIP. The latter contains repository documentation, not the full experimental artifact.

## Inspect and replay

Extract the artifact ZIP and open its `README.md` and `START_HERE.md`. The public derivative offline entry is:

```text
python -B reproduce_review.py
```

It requires Python 3.10 or newer and operates on archived evidence. It does not build or start a controller, require EtherCAT hardware, or execute the legacy FK unit-test routine. Do not execute archived acquisition/controller runners as part of this entry. The original-byte-only integrity stage is not applicable after redaction; the public entry checks its distributed manifest instead. The documented replay recomputes specified historical relations and verdicts; it does not certify producer meaning or historical loaded binaries.

No new controller run, experiment, project test, or independent non-author replication was performed for this publication. Historical replay results remain identified as historical, AI-assisted checks in the author workspace.

## Navigate the current paper

`CURRENT_CLAIM_EVIDENCE_LOCK.csv` maps the refocused manuscript to the original evidence IDs and release-relative paths. `NEW_FRONTMATTER_CLAIM_MAP.csv` covers its revised abstract and conclusion. Original RQ1–RQ5 identifiers remain unchanged in archived protocols. Current Q1–Q3 reorganize interpretation without pooling or renumbering experiments.

- Q1: G93 output masking and pose position/orientation information.
- Q2: native producer selection, binding review, qualification, and source-misbinding comparisons.
- Q3: LinuxCNC/pose instantiation, evidence gaps, and verdict-policy cost.

The generic reference's 120/120 eligible parity, five conclusive FAILs withheld by mandatory witnesses, source-informed STRONG parity, and incomplete evidence chains remain reported.

## Public-edition scope

The original reviewer package remains unchanged in the author's archive. In this public edition, the ND2410 archive omits its `source/transport.git/` transfer repository, including temporary Git packs. The pilot archive also omits two native executable snapshots; their original hashes remain documented. Numerical observations and expected verdicts are preserved; files containing local environment metadata are explicitly redacted and have new distributed hashes. `PUBLIC_EDITION_CHANGES.csv`, `ND2410_PUBLIC_MEMBER_MAP.csv`, `PILOT_PUBLIC_MEMBER_MAP.csv`, and the retained original manifest document the packaging difference. The public root manifest describes the distributed bytes; it must not be confused with the original reviewer-package manifest.

The public release does not include the unpublished manuscript, internal editorial approval files, account credentials, or the working CNC development checkout. Local usernames, host names, home/workspace paths and process identities are redacted or pseudonymized. See PRIVACY_AND_REDACTION.md and SANITIZATION_MANIFEST.csv. The private reverse mapping is not public.

## Rights and third-party material

See [NOTICE.md](NOTICE.md) and [THIRD_PARTY/README.md](THIRD_PARTY/README.md). Public access is not a blanket open-source license for every component. Original research materials retain their authors' rights; upstream LinuxCNC excerpts and patches retain their applicable upstream terms. The upstream GPL-2.0 text and source locations are provided. Historical reviewer-only notices are retained as records of the earlier distribution, rather than a claim that the old package was already public.

## Evidence boundaries

Pose uses sampled commanded-joint forward kinematics, not physical TCP metrology. LinuxCNC LC-D1 source-assisted misbinding adjudication, seeded LC-T violations, and the upstream-reported LC-ND2410 defect are distinct evidence mechanisms. Hashes establish byte identity, not complete source-to-binary/load truth. HBES-N1 remains registry-only; the completeness pilot closes no full qualification chain. No population incidence, new monitoring expressiveness, or measured engineering-effort advantage is claimed.

This release has no DOI. External access verification is reported separately from independent experimental replication.
