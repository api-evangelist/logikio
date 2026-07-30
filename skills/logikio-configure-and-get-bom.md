---
name: Configure a product and retrieve its BOM (Runtime v2)
description: Start a Logik.io configuration, apply field selections, save it, then pull the Sales Bill of Materials.
api: openapi/logikio-runtime-v2-openapi-original.yml
operations: [startConfigV2, updateConfigByUuidV2, getConfigByUuidV2, getSalesBomV2]
method: generated
generated: '2026-07-20'
---

# Configure a product and retrieve its BOM

Use the Logik.io Runtime v2 Configuration API to configure a product and get its Bill of Materials.

## Auth
- Send `Authorization: Bearer <Runtime Token>` on every request (create the token in Logik.io Admin > Runtime Clients).
- Send an `Origin` header that is allow-listed for that Runtime Client, or the call is rejected (403).
- Use the v2 media type: `Content-Type: application/vnd.logik.cfg-v2+json` and matching `Accept`.

## Steps
1. **Start a configuration** — `startConfigV2` (`POST /api`). Provide the product/blueprint to configure. The response returns a configuration `uuid` and the current field state (`ConfigResponseV2`).
2. **Apply selections** — `updateConfigByUuidV2` (`PATCH /api/{uuid}`) with the fields to set. Inspect the returned `Message[]` array; any entry with `error: true` is a blocking rule/validation message on the named `field`.
3. **Save** — call `updateConfigByUuidV2` with `?save` when the configuration is complete and valid.
4. **Read state (optional)** — `getConfigByUuidV2` (`GET /api/{uuid}`) to re-fetch the configuration.
5. **Get the BOM** — `getSalesBomV2` (`GET /api/{uuid}/bom/sales`) for the Sales BOM (or `getAllBomV2` for the full BOM, `getManufacturingBomV2` for manufacturing).

## Rules
- Pagination on Admin list endpoints uses `page`/`limit`/`sort` (see conventions/logikio-conventions.yml).
- There is no idempotency-key contract; mutation is UUID-addressed via PATCH, so re-PATCHing the same `uuid` is the safe retry path.
- Errors return `{ errorMessage, timestamp }` (see errors/logikio-problem-types.yml).
