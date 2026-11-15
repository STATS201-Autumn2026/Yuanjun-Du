# Senior Work extension: robot metrics and deployment value

STATS 201 PS1 pilot, Yuanjun Du, 15 November 2026.

The broader thesis asks which world-model diagnostics add predictive value beyond operating capacity for financial and resource outcomes. The existing controlled demo paper is a foundation. This course pilot audits public annotation availability before extending to grouped prediction and external validation.

## Reproduce
Python 3.10+; standard library only; no pip install required.
```sh
python3 audit.py
```
The script materializes a byte-pinned local source snapshot if absent, then writes audit_result.json. Expected: 116 category rows; 0/1/2/3 nonblank slots = 1/4/50/61; 115 label-bearing rows; 287 populated slots; Kitchenware empty. Missing is not false. This is an annotation audit, not a VLM accuracy, execution, or economic experiment.

## Data and versions
Course shared source: https://huggingface.co/datasets/DKU-STATS201-Autumn2026/pacbench-QL/tree/c14b0f79dbb7dddb3ee1c21fb1280091a30d233f
Upstream: https://huggingface.co/datasets/lens-lab/pacbench
Personal copy: https://huggingface.co/datasets/YuanjunDu/pacbench-QL/tree/8905a9701f1f492fe2ccd0cea5018e503272df6e
The source CSV was retained on 2026-11-07; SHA-256 b9da6d6f7e7902c55523291b0c256734f9c9a37cae66a5c75adbf6efccac87c8. It has not been byte-matched to the pinned remote snapshot in this session. Repository commit history identifies the exact code revision. The derived per-category release card is prepared locally; do not assume that it has been published on HF.

## Rights and limitations
Upstream HF card declares MIT. No photographs are redistributed by this pilot. Category annotations are not image-level negatives, complete affordance lists, actual robot outcomes or observed firm accounts. Review upstream component rights before enlarging the release.

PAC Bench: Gundawar, Sagar and Senanayake (2025), NeurIPS Datasets and Benchmarks. https://arxiv.org/abs/2506.23725

## Assistance
Codex assisted drafting, audit implementation and checking under instructor permission reported by the student. Student review and defense remain required.

## Published derived dataset
https://huggingface.co/datasets/DKU-STATS201-Autumn2026/yuanjun-du-robot-metrics-pilot/tree/c7d816d87accfdb4c412a35a8a45faeb00a9e51e
This release is published and includes the derived table, card and audit script. Download this exact revision. The audit script also regenerates category_audit.csv.
