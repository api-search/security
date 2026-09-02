---
api_key_in: []
api_specs:
- filename: stotles-buyers-api-openapi.yml
  format: yaml
  label: Stotles Buyers API
  slug: stotles-buyers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-buyers-api-openapi.yml
- filename: stotles-frameworks-api-openapi.yml
  format: yaml
  label: Stotles Frameworks API
  slug: stotles-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-frameworks-api-openapi.yml
- filename: stotles-notices-api-openapi.yml
  format: yaml
  label: Stotles Notices API
  slug: stotles-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-notices-api-openapi.yml
- filename: stotles-suppliers-api-openapi.yml
  format: yaml
  label: Stotles Suppliers API
  slug: stotles-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-suppliers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Stotles Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stotles declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Stotles
provider_slug: stotles
scheme_count: 1
schemes:
- applies_to:
  - https://api.stotles.com/v1 (all 8 operations — global `security` requirement in the spec)
  - https://api.stotles.com/mcp (MCP server; same header per the endpoint's own self-description)
  description: '"Every request needs an API key, sent in the `x-api-key` header. Keys are issued by Stotles — ask your Customer Success Manager. A key identifies your organization, so treat it as a secret: keep it server-side and out of source control. Requests without a valid key get a 401." — Stotles Public API, info.description.'
  example_request: "curl -G https://api.stotles.com/v1/notices/search \\\n  -H \"x-api-key: $STOTLES_API_KEY\" \\\n  --data-urlencode \"query=cyber security\"\n"
  id: apiKey
  in: header
  name: x-api-key
  required: true
  type: apiKey
slug: stotles-authentication
source_filename: stotles-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  openapi/stotles-public-api-openapi.yml components.securitySchemes (harvested verbatim from\n  https://api.stotles.com/v1/openapi.json), the Authentication section of the spec's own\n  info.description, and a live unauthenticated probe of\n  https://api.stotles.com/v1/notices/search (HTTP 401, application/problem+json).\ndocs: https://api.stotles.com/v1/openapi.json\nsummary: >-\n  One scheme, one header, no OAuth, no scopes, no token exchange. Every request to the Stotles\n  Public API and to the Stotles MCP server carries a long-lived static API key in `x-api-key`.\n  Keys are issued out of band by a Stotles Customer Success Manager; there is no self-serve\n  key issuance and no developer console.\n\nschemes:\n  - id: apiKey\n    type: apiKey\n    in: header\n    name: x-api-key\n    required: true\n    applies_to:\n      - https://api.stotles.com/v1 (all 8 operations — global `security` requirement in the spec)\n  \
  \    - https://api.stotles.com/mcp (MCP server; same header per the endpoint's own self-description)\n    description: >-\n      \"Every request needs an API key, sent in the `x-api-key` header. Keys are issued by Stotles —\n      ask your Customer Success Manager. A key identifies your organization, so treat it as a\n      secret: keep it server-side and out of source control. Requests without a valid key get a\n      401.\" — Stotles Public API, info.description.\n    example_request: |\n      curl -G https://api.stotles.com/v1/notices/search \\\n        -H \"x-api-key: $STOTLES_API_KEY\" \\\n        --data-urlencode \"query=cyber security\"\n\noauth2:\n  supported: false\n  evidence:\n    - 'openapi components.securitySchemes declares only `apiKey`; no oauth2 or openIdConnect scheme.'\n    - 'https://api.stotles.com/.well-known/oauth-authorization-server -> 404'\n    - 'https://api.stotles.com/.well-known/oauth-protected-resource -> 404'\n    - 'https://app.stotles.com/.well-known/openid-configuration\
  \ -> 404'\n  note: >-\n    No OAuth means no scopes artifact for this provider — scopes/ is genuinely N/A, not missing.\n    Enterprise SSO is offered on the Expert tier for human login to app.stotles.com per the pricing\n    page, but no OpenID Provider metadata is published and SSO does not extend to the API.\n\nmutual_tls:\n  supported: false\nwebhooks_signing:\n  supported: false\n  note: No webhook or event surface is published; nothing to sign. See lifecycle/ and apis.yml.\n\nkey_properties:\n  identity_granularity: organization\n  note: '\"A key identifies your organization\" — one key represents a tenant, not an end user.'\n  rotation_policy:\n    published: false\n    note: >-\n      No documented rotation cadence, expiry, revocation endpoint, or multi-key support. There is no\n      published way for a customer to rotate a leaked key themselves; the documented channel for\n      anything key-related is the Customer Success Manager.\n  prefix:\n    published: false\n    note:\
  \ >-\n      Stotles does not publish a key prefix (contrast Stripe `sk_live_`). Because there is no\n      documented prefix and no test-mode key, a leaked Stotles key is not recognizable by shape to\n      secret-scanning tooling — neither GitHub push protection nor this pipeline's sanitizer can\n      match it.\n  test_mode:\n    exists: false\n    note: >-\n      No sandbox, test key, or test mode is published. The only key is a live key against production\n      data. See the absent sandbox/ artifact — this is a real DX gap, not an omission by us.\n\nfailure_semantics:\n  missing_or_invalid_key:\n    http_status: 401\n    content_type: application/problem+json\n    body_observed: >-\n      {\"type\":\"https://api.stotles.com/problems/unauthenticated\",\"title\":\"Unauthenticated\",\n      \"status\":401,\"detail\":\"Missing or invalid API key.\"}\n    probed: '2026-08-14 against https://api.stotles.com/v1/notices/search?query=cyber (no key sent)'\n  mcp_missing_key:\n    http_status:\
  \ 401\n    transport: json-rpc\n    body_observed: >-\n      {\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Unauthorized: Missing API key\"},\"id\":null}\n    probed: '2026-08-14 against POST https://api.stotles.com/mcp (tools/list, no key sent)'\n    note: >-\n      The MCP surface reports auth failure as a JSON-RPC error object with code -32001, NOT as an\n      RFC 9457 problem document. An agent handling both surfaces needs two error paths.\n\nagent_notes:\n  - >-\n    Static header key, no refresh, no expiry: an agent needs exactly one secret and never has to\n    implement a token lifecycle. That is the ergonomic upside of this design.\n  - >-\n    The downside is procurement: there is no self-serve signup for a key. An agent builder cannot\n    obtain credentials without a commercial conversation with Stotles. See\n    plans/stotles-plans-pricing.yml — API access is not attached to any published tier.\n  - >-\n    Send the key server-side only. It carries the whole\
  \ organization's entitlement and there is no\n    documented scoping, rate-limit partitioning per user, or revocation self-service.\n\ncross_references:\n  conventions: conventions/stotles-conventions.yml\n  errors: errors/stotles-problem-types.yml\n  rate_limits: rate-limits/stotles-rate-limits.yml\n  mcp: mcp/stotles-mcp.yml\n  well_known: well-known/stotles-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/authentication/stotles-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Procurement
- Public Sector
- Government
- Tenders
- Sales Intelligence
- B2G
- Market Intelligence
- OpenAPI
- MCP
- agent-native
- Contract Awards
- Framework Agreements
- CPV
- United Kingdom
- Ireland
- GovTech
---
