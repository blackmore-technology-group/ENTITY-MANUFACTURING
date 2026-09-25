# ENTITY-MANUFACTURING

**ENTITY v3.4.0 executable Manufacturing implementation package.**

**Current core compatibility:** ENTITY v3.4.1 — Protocol Origin Lineage & Sovereign User Bootstrap. The sealed domain-package payload remains v3.4.0 and was requalified unchanged against v3.4.1.

This repository configures the **one ENTITY Global Passport** for manufacturing and industrial workflows. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.1 core release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.1) · [Global Passport documentation](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/GLOBAL_PASSPORT.md) · [Domain packages](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/DOMAIN_PACKAGES.md)

## What this package is for

Use ENTITY-MANUFACTURING as the starting point when you need a governed passport and continuous-provenance layer around industrial assets, components, production records, telemetry or derived outputs while keeping authority, rights, evidence and custody explicit.

The v3.4 package includes mappings for **OPC UA** and **Asset Administration Shell (AAS)**. Those mappings describe correspondence; ENTITY does not redefine the external standards.

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

The verifier checks the repository inventory and the package/source-release binding.

## Release binding

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `bc29a0de024cea22552078ff1913fa3df2b189436cb853cc2f4e08974325c4bc`

## Go deeper

- [ENTITY v3.4.1 core](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.1)
- [Developer portal](https://github.com/blackmore-technology-group/ENTITY/blob/main/DEVELOPERS.md)
- [Engineering evidence](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/ENGINEERING_EVIDENCE.md)
- [Open contributor tasks](https://github.com/blackmore-technology-group/ENTITY/issues?q=is%3Aissue+is%3Aopen)

## Truth and compliance boundary

External standards remain externally authoritative and are mapped, not redefined. Package verification does **not** establish regulatory compliance, objective external truth, legal title or accounting fair value. Provider custody does not create ENTITY authority.

Deployment-specific safety, legal, security, standards-conformance and operational determinations remain the responsibility of the deploying organization.
