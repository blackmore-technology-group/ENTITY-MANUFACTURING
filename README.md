# ENTITY-MANUFACTURING

**Sealed ENTITY v3.4.0 Manufacturing implementation package, evaluated in the current ENTITY v3.4.2 ecosystem.**

**Current canonical core release:** [ENTITY v3.4.2 — Canonical BTDU Release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2).

The sealed domain-package payload in this repository remains the historical v3.4.0 package. Its recorded package-specific requalification against v3.4.1 remains historical evidence; this README does not rewrite that evidence into a new v3.4.2 package qualification. The current v3.4.2 adoption path is open for clean-clone external evaluation.

This repository configures the **one ENTITY Global Passport** for manufacturing and industrial workflows. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.2 release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2) · [ENTITY documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/) · [Manufacturing domain documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/domains/manufacturing.html) · [Domain-package evaluation task](https://github.com/blackmore-technology-group/ENTITY/issues/46)

## What this package is for

Use ENTITY-MANUFACTURING as the starting point when you need a governed passport and continuous-provenance layer around industrial assets, components, production records, telemetry or derived outputs while keeping authority, rights, evidence and custody explicit.

The sealed package includes mappings for **OPC UA** and **Asset Administration Shell (AAS)**. Those mappings describe correspondence; ENTITY does not redefine the external standards.

Typical evaluation paths include:

- maintaining provenance across component, asset and production-state changes;
- binding scoped authority and rights to industrial digital records;
- preserving evidence across suppliers, platforms or custodians without turning infrastructure possession into authority;
- composing jurisdiction, industry, trust and technical profiles inside one Global Passport.

## Deploy the package

Required deployment facts:

- `organization`
- `jurisdiction`
- `authority_source`
- `asset_namespace`

`deployment.example.json` is intentionally non-production until every `CONFIGURE-ME` value is replaced with organization-specific facts.

```text
Select package → configure organization facts → connect systems/data → ingest → verify passport → run conformance → deploy
```

## Verify locally

```bash
python tools/verify_package.py
```

The verifier checks repository inventory and the sealed package/source-release binding. A successful package verification does not, by itself, establish a new v3.4.2 qualification claim.

## Sealed package provenance

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `bc29a0de024cea22552078ff1913fa3df2b189436cb853cc2f4e08974325c4bc`

These values describe the sealed historical package payload and should not be rewritten merely because the current core release advances.

## Current evaluation path

- [ENTITY v3.4.2 core release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2)
- [Manufacturing domain manual](https://blackmore-technology-group.github.io/ENTITY-DOCS/domains/manufacturing.html)
- [Data lineage vs provenance vs rights](https://blackmore-technology-group.github.io/ENTITY-DOCS/guides/data-lineage-vs-provenance-rights.html)
- [Standards mapping](https://blackmore-technology-group.github.io/ENTITY-DOCS/developer/standards-mapping.html)
- [Try one current domain-package path from a clean clone](https://github.com/blackmore-technology-group/ENTITY/issues/46)
- [External verification challenge](https://github.com/blackmore-technology-group/ENTITY/issues/55)

## Truth and compliance boundary

External standards remain externally authoritative and are mapped, not redefined. Package verification does **not** establish regulatory compliance, objective external truth, legal title or accounting fair value. Provider custody does not create ENTITY authority.

Deployment-specific safety, legal, security, standards-conformance and operational determinations remain the responsibility of the deploying organization.
