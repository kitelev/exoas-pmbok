---
exo__Asset_isDefinedBy: "[[58df7855-d5fc-4f7c-9fa5-d909a1749b7e]]"
exo__Asset_uid: b74ed0df-bd71-48d2-8dfc-bef0aa2be60e
exo__Asset_createdAt: 2026-05-31T16:51:53
exo__Asset_updatedAt: 2026-05-31T16:51:53
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76]]"
exo__Instance_class:
  - "[[ff1b9be3-9ffd-4d15-aa73-7e8ed94fe9bf]]"
exo__Asset_label: "R6 — iPhone partial sync collisions (broken wikilinks из in-focus → excluded)"
aliases:
  - "R6 — iPhone partial sync collisions"
pmbok__RiskItem_project: "[[2bd5e308-07c8-4124-9a9b-5ebb08725a22|RFC b6ba5595 — exo__FocusProfile implementation]]"
pmbok__RiskItem_status: "[[399f782c-fa79-4dff-a029-adca5ac700e5]]"
pmbok__RiskItem_probability: "[[85abeb12-0f64-4b32-8a87-df62d3fea544|pmbok__RiskProbabilityMedium]]"
pmbok__RiskItem_impact: "[[2d71e4bf-7e7f-45d9-9a46-3b7815e63715|pmbok__RiskImpactLow]]"
pmbok__RiskItem_mitigationSummary: "Phase 5 sparse-checkout config; broken wikilinks отображаются Obsidian'ом как обычные unresolved links (existing behavior). Phase 5 scope deferred — risk lives until Phase 5 ships."
exo__Asset_relates:
  - "[[b6ba5595-7675-4fe7-b521-272246d8d710|RFC: exo__FocusProfile — lazy-loaded ontology selection per device]]"
---

# R6 — iPhone partial sync collisions

Working Copy не sync'нул submodule, но wikilink из in-focus asset ссылается на assets из excluded submodule → broken wikilinks в Obsidian on iPhone.

Impact Low: Obsidian handles unresolved wikilinks gracefully (existing behavior — clickable но не resolve). User experience не критично affected, но noisy.
