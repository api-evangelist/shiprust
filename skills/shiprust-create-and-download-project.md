---
name: shiprust-create-and-download-project
description: Create a new project and then download its generated zip file.
api: openapi/shiprust-openapi.json
operations:
- create_project
- download_project
generated: '2026-10-20'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/shiprust-openapi.json ; every operationId checked against the contract
---

# shiprust-create-and-download-project

Create a new project and then download its generated zip file.

## Steps

1. 1. `create_project` – send a POST request to `/api/v1/projects` with the required request body fields (as defined by the new‑project form).
2. 2. `download_project` – send a GET request to `/api/v1/projects/{id}/download` using the project ID returned from the previous step.

## Rules

- Authentication: include the API key in the `Authorization` header as required by the `api_key` scheme.
- Path parameters: `{id}` must be supplied for `download_project`.
