---
anonymous_access: true
api_key_in: []
api_specs:
- filename: convalytics-dev-ingest-api-openapi.yml
  format: yaml
  label: Convalytics Ingest API
  slug: convalytics-dev-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convalytics-dev/openapi/convalytics-dev-ingest-api-openapi.yml
- filename: convalytics-dev-meta-api-openapi.yml
  format: yaml
  label: Convalytics Meta API
  slug: convalytics-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convalytics-dev/openapi/convalytics-dev-meta-api-openapi.yml
- filename: convalytics-dev-provision-api-openapi.yml
  format: yaml
  label: Convalytics Provision API
  slug: convalytics-dev-provision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convalytics-dev/openapi/convalytics-dev-provision-api-openapi.yml
- filename: convalytics-dev-verify-api-openapi.yml
  format: yaml
  label: Convalytics Verify API
  slug: convalytics-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convalytics-dev/openapi/convalytics-dev-verify-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Convalytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convalytics declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Convalytics
provider_slug: convalytics-dev
scheme_count: 3
schemes:
- description: Public, non-secret write key (wk_...) identifying one project. Write-only, cannot read data, safe to ship in client code; revocable from the dashboard. Sent as the writeKey JSON field on POST /ingest and POST /ingest/batch, the ?writeKey= query parameter on GET /verify, and ?key= on the browser script.
  in: body / query
  name: writeKey
  operations:
  - ingestEvent
  - ingestBatch
  - verifyWriteKey
  - getTrackingScript
  quote: There are no scopes, no token exchange, no refresh flow. One write key, one project, write-only.
  type: apiKey
- description: POST /api/provision requires no auth and returns a fresh write key plus a claimUrl; capped at 5 unclaimed projects per IP per hour.
  name: none
  operations:
  - provisionProject
  - getHealth
  - getLlmsTxt
  type: none
- description: The MCP server (https://api.convalytics.dev/mcp) uses an API token (Authorization Bearer cnv_...) generated at https://convalytics.dev/tokens with scope read (default) or write (funnel-mutating tools). Tokens bind to one team. Not used by the REST ingestion API. MCP endpoint gated to Solo and Pro plans (402 plan_required on Free).
  name: mcpBearerToken
  scheme: bearer
  token_scopes:
  - read
  - write
  type: http
slug: convalytics-dev-authentication
source_filename: convalytics-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convalytics.dev/llms-full.txt\ndocs: https://convalytics.dev/llms-full.txt\nschemes:\n- name: writeKey\n  type: apiKey\n  in: body / query\n  description: Public, non-secret write key (wk_...) identifying one project. Write-only, cannot read data, safe to ship in client code; revocable from the dashboard. Sent as the writeKey JSON field on POST /ingest and POST /ingest/batch, the ?writeKey= query parameter on GET /verify, and ?key= on the browser script.\n  operations: [ingestEvent, ingestBatch, verifyWriteKey, getTrackingScript]\n  quote: There are no scopes, no token exchange, no refresh flow. One write key, one project, write-only.\n- name: none\n  type: none\n  description: POST /api/provision requires no auth and returns a fresh write key plus a claimUrl; capped at 5 unclaimed projects per IP per hour.\n  operations: [provisionProject, getHealth, getLlmsTxt]\n- name: mcpBearerToken\n  type: http\n  scheme: bearer\n\
  \  description: The MCP server (https://api.convalytics.dev/mcp) uses an API token (Authorization Bearer cnv_...) generated at https://convalytics.dev/tokens with scope read (default) or write (funnel-mutating tools). Tokens bind to one team. Not used by the REST ingestion API. MCP endpoint gated to Solo and Pro plans (402 plan_required on Free).\n  token_scopes: [read, write]\nnotes: The OpenAPI declares no securitySchemes; the write key is a request body/query field. Dashboard sign-in uses Convex Auth with Google OAuth and is separate from the API. Docs state \"Not in v1 ... OAuth\" for MCP.\n"
source_yaml_url: https://artifacts.apis.io/convalytics-dev/authentication/convalytics-dev-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Analytics
- Product Analytics
- Web Analytics
- Convex
- Event Tracking
- MCP
- Developer Tools
---
