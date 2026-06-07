---
exo__Asset_isDefinedBy: "[[58df7855-d5fc-4f7c-9fa5-d909a1749b7e]]"
exo__Asset_uid: a3e82dcb-fd6d-4ece-bc61-b9f103fd49db
exo__Asset_createdAt: 2026-05-16T13:02:15+0500
exo__Asset_updatedAt: 2026-05-16T13:02:15+0500
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76]]"
exo__Instance_class:
  - "[[985f6c53-5925-4b03-9c2b-202b196d11a2]]"
exo__Asset_label: "Phase 2 Charter — Measurement #1 (decision gate)"
aliases:
  - "Charter — Phase 2 gate"
  - "Чартер — Фаза 2 замер"
pmbok__ProjectCharter_project: "[[e0c1a23b-4ffc-4029-8e5b-fc40e8210cce]]"
pmbok__ProjectCharter_authorizedBy: "[[0aa339bc-9b56-400a-8148-cbde57bbf0b6]]"
exo__Asset_relates:
  - "[[5003ef6f-fe89-456c-a1e9-19b475bf4f5e]]"
---

# Phase 2 Charter — Measurement #1 (decision gate)

> **Delivery boundary** (PCS 3/4). Distinct AC: decision matrix triggers downstream phase scope. Root baseline: [[dedf9460-a821-42c0-a31b-e448def51b0f]].

## 1. Scope
**IN:** Recreate `/tmp/unbiased-baseline-50.jsonl` (seed=42), run `measure-recall.py`, manually classify, compute Recall@5 + Wilson 95 % LB, apply 3-way decision matrix.

**OUT:** Any structural changes к graph (только measurement).

## 2. Decision Matrix (AC)
- **Recall@5 ≥ 50 %** → SKIP Phase 3 (de-stamping risky if not needed), jump to Phase 4
- **25-50 %** → continue Phase 3 → 4 → 5 → 6 (full sequence)
- **< 25 %** → STOP, escalate to user; orphan stamping ineffective hypothesis

## 3. Constraints
- Reproducibility: seed=42 mandatory
- Same classification scheme как baseline doc 2026-05-09
- No graph modifications during measurement window

## 4. Budget
- 30 минут wall-time
- User decision required
- Owner: a.kitelev (gate authority)
