---
api_key_in: []
api_specs:
- filename: millimetric-openapi.yml
  format: yaml
  label: Millimetric Analytics API
  slug: millimetric-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/millimetric/refs/heads/main/openapi/millimetric-openapi.yml
auth_types:
- http
description: Millimetric uses Bearer API keys of the form {kind}_{env}_{prefix}_{secret}, modelled on Stripe's pk_/sk_ split. Four key kinds map to two scopes (ingest, read) plus an account-level read variant. pk_* keys are browser-safe and origin-allowlisted; sk_/rk_/ak_ are server-side. Not OAuth — there is no OAuth2/OIDC surface, so there is no scopes/ artifact.
kind: authentication
layout: security
method: searched
name: Millimetric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Millimetric secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Millimetric
provider_slug: millimetric
scheme_count: 1
schemes:
- format: '{kind}_{env}_{prefix}_{secret}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/millimetric-openapi.yml
  type: http
slug: millimetric-authentication
source_filename: millimetric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.millimetric.ai/core-concepts/api-keys.md\ndocs: https://docs.millimetric.ai/core-concepts/api-keys.md\ndescription: >-\n  Millimetric uses Bearer API keys of the form {kind}_{env}_{prefix}_{secret}, modelled on\n  Stripe's pk_/sk_ split. Four key kinds map to two scopes (ingest, read) plus an\n  account-level read variant. pk_* keys are browser-safe and origin-allowlisted; sk_/rk_/ak_\n  are server-side. Not OAuth — there is no OAuth2/OIDC surface, so there is no scopes/ artifact.\nsummary:\n  types: [http]\n  scheme: bearer\n  oauth2_flows: []\n  api_key_kinds: [pk_, sk_, rk_, ak_]\n  scopes: [ingest, read, account-read]\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    format: '{kind}_{env}_{prefix}_{secret}'\n    sources: [openapi/millimetric-openapi.yml]\nkey_kinds:\n  - kind: pk_\n    scope: ingest\n    surface: Browsers, public pages, snippets\n    origin_allowlisted: true\n    notes:\
  \ Ingest only. Rejected at /mcp. Requires an Origin header in the project's allowed_origins.\n  - kind: sk_\n    scope: ingest + read\n    surface: Servers, cron jobs, MCP write access\n    origin_allowlisted: false\n    notes: Required for /v1/forget. Accepted by /mcp.\n  - kind: rk_\n    scope: read\n    surface: Server-side dashboards, MCP clients (recommended)\n    notes: Read only (query/stats/sources + MCP read tools). Cannot ingest. Recommended for AI agents.\n  - kind: ak_\n    scope: account-read\n    surface: Account-level MCP (/mcp/account) — agencies, multi-product teams\n    plan: Business\n    notes: Reads every project the account owns through one credential. Cannot ingest.\nstorage:\n  secret: Shown once at mint; only sha256(secret || pepper) stored. Not recoverable.\n  prefix: 8-char lookup key, safe to display.\n  caching: Worker caches verified keys 5 minutes per instance; revocation takes effect within that window.\n  last_used_at: updated on each successful auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/millimetric/refs/heads/main/authentication/millimetric-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Analytics
- Web Analytics
- Product Analytics
- Attribution
- Privacy
- MCP
- AI Agents
- Events
- Developer Tools
---
