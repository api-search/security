---
api_key_in:
- body
- query
api_specs:
- filename: event-registry-articles-api-openapi.yml
  format: yaml
  label: Event Registry Articles API
  slug: event-registry-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-articles-api-openapi.yml
- filename: event-registry-events-api-openapi.yml
  format: yaml
  label: Event Registry Events API
  slug: event-registry-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-events-api-openapi.yml
- filename: event-registry-suggest-api-openapi.yml
  format: yaml
  label: Event Registry Suggest API
  slug: event-registry-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-suggest-api-openapi.yml
- filename: event-registry-topic-pages-api-openapi.yml
  format: yaml
  label: Event Registry Topic Pages API
  slug: event-registry-topic-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-topic-pages-api-openapi.yml
- filename: event-registry-usage-api-openapi.yml
  format: yaml
  label: Event Registry Usage API
  slug: event-registry-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Event Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Event Registry secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Event Registry
provider_slug: event-registry
scheme_count: 1
schemes:
- alternate_transmission: query parameter
  description: 'A single long-lived API key. The provider''s own client injects it as an `apiKey` member of the JSON POST body on every request; a query parameter of the same name is also accepted. There is no Authorization header form.

    '
  evidence: 'newsapi-mcp src/client.ts request(): `const payload: Record<string, unknown> = { apiKey };` merged into the body of a POST to `${BASE_URL}${path}` with `headers: { "Content-Type": "application/json" }` and no auth header.

    '
  header: null
  in: body
  name: apiKeyAuth
  parameter: apiKey
  primary_transmission: JSON POST body field
  sources:
  - https://github.com/EventRegistry/newsapi-mcp/blob/main/src/client.ts
  - openapi/event-registry-articles-api-openapi.yml
  - openapi/event-registry-events-api-openapi.yml
  - openapi/event-registry-suggest-api-openapi.yml
  - openapi/event-registry-topic-pages-api-openapi.yml
  - openapi/event-registry-usage-api-openapi.yml
  type: apiKey
slug: event-registry-authentication
source_filename: event-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >\n  https://raw.githubusercontent.com/EventRegistry/newsapi-mcp/main/src/client.ts and\n  src/types.ts — Event Registry's own published first-party client, read 2026-08-13 — plus\n  the securitySchemes declared in openapi/event-registry-*-openapi.yml. The documentation\n  portal at https://newsapi.ai/documentation is JavaScript-rendered and returns only an SPA\n  shell to a machine fetch, so the provider's open-source client is the authoritative\n  readable description of how authentication actually works.\ndocs: https://newsapi.ai/documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - body\n  - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  bearer_token: false\n  scoped: false\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: body\n  parameter: apiKey\n  description: >\n    A single long-lived API key. The provider's own client injects it as an `apiKey` member\n    of the JSON POST body\
  \ on every request; a query parameter of the same name is also\n    accepted. There is no Authorization header form.\n  primary_transmission: JSON POST body field\n  alternate_transmission: query parameter\n  header: null\n  evidence: >\n    newsapi-mcp src/client.ts request(): `const payload: Record<string, unknown> = { apiKey };`\n    merged into the body of a POST to `${BASE_URL}${path}` with\n    `headers: { \"Content-Type\": \"application/json\" }` and no auth header.\n  sources:\n  - https://github.com/EventRegistry/newsapi-mcp/blob/main/src/client.ts\n  - openapi/event-registry-articles-api-openapi.yml\n  - openapi/event-registry-events-api-openapi.yml\n  - openapi/event-registry-suggest-api-openapi.yml\n  - openapi/event-registry-topic-pages-api-openapi.yml\n  - openapi/event-registry-usage-api-openapi.yml\nacquisition:\n  url: https://newsapi.ai/register\n  self_serve: true\n  credit_card_required: false\n  free_allocation: 2,000 searches (one-time, last 30 days of data, non-commercial)\n\
  \  approval_required: false\nkey_properties:\n  prefix: none\n  format: not published\n  expiry: not published\n  rotation: not published\n  multiple_keys: not published\n  environment_separation: false\n  environment_note: >\n    One key for everything. There is no test-mode key and no sandbox host — see\n    sandbox/event-registry-sandbox.yml.\nscopes:\n  supported: false\n  note: >\n    No OAuth scopes, no permission model, no per-key restriction. A key carries the full\n    entitlement of its plan. derive-oauth-scopes.py returned zero oauth2 schemes on\n    2026-08-13, so no scopes artifact is emitted.\nmcp_authentication:\n  mechanism: environment variable\n  variable: NEWSAPI_KEY\n  transport: stdio (local)\n  oauth: false\n  note: >\n    The first-party MCP server takes the same API key via NEWSAPI_KEY and forwards it in the\n    request body. No OAuth handshake, no /.well-known/oauth-protected-resource — both hosts\n    returned the SPA shell for every OAuth discovery path probed.\n\
  failure_modes:\n  - status: 401\n    meaning: Missing, malformed or invalid key.\n  - status: 403\n    meaning: >\n      Classified as an auth error by the provider's own client. In practice a valid key\n      lacking entitlement — for example historical archive depth beyond the free plan's\n      30-day window.\nsecurity_notes:\n  - >\n    Because the key is normally carried in a POST body it stays out of server access logs and\n    Referer headers. The API also accepts it as a query parameter, however, so a careless\n    integrator can still leak it into logs and browser history.\n  - >\n    A long-lived, unscoped, non-expiring, non-rotatable bearer of full plan entitlement is the\n    weakest common credential shape. There is no documented revocation or rotation procedure.\n  - >\n    No security.txt and no vulnerability disclosure program were found — see\n    well-known/event-registry-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/authentication/event-registry-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Media Monitoring
- News Intelligence
- Event Detection
- Named Entity Recognition
- Sentiment Analysis
- Media Analytics
- News API
---
