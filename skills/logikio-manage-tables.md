---
name: Manage a Logik.io managed data table (Admin API)
description: Create a managed table, define columns, load rows or CSV, and export the table data.
api: openapi/logikio-admin-managed-tables-openapi-original.yml
operations: []
method: generated
generated: '2026-07-20'
---

# Manage a Logik.io managed data table

Use the Logik.io Admin Managed Tables API to create and populate the lookup/pricing tables that rules reference.

## Auth
- Send `Authorization: Bearer <Admin Token>` (register the key in Logik.io Admin > Utilities > Admin API Keys).

## Steps
1. **List tables** — `GET /api/managedTables/v1/managedTables` to see existing tables (supports `page`/`limit`/`sort`).
2. **Create a table** — `POST /api/managedTables/v1/managedTables` with the table name and column metadata.
3. **Add / adjust columns** — `PATCH /api/managedTables/v1/managedTables/{tableName}/metadata/columns` to add or remove columns; `DELETE .../metadata/columns/{columnName}` to drop one.
4. **Load data** — add rows one at a time with `POST /api/managedTables/v1/managedTables/{tableName}`, or bulk-load with `POST /api/managedTables/v2/managedTables/{tableName}` (CSV upload) / `PUT` to replace all data.
5. **Read a row** — `GET /api/managedTables/v1/managedTables/{tableName}/{rowId}`; update with `PATCH`, delete with `DELETE`.
6. **Export** — `POST /api/managedTables/v3/managedTables/{tableName}/export` returns a `jobId`; poll `GET /api/managedTables/v2/job/{tableExportJobId}` until complete, then download via `GET /api/managedTables/v2/job/{tableExportJobId}/file`.

## Rules
- Export is async/job-based — poll the job before downloading (see data-model/logikio-data-model.yml Job entity).
- Errors return `{ errorMessage, timestamp }` (see errors/logikio-problem-types.yml).

> Note: operations in this spec have no `operationId` fields; steps reference the verbatim method+path from openapi/logikio-admin-managed-tables-openapi-original.yml.
