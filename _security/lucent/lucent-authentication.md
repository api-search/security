---
api_key_in:
- header
- query
api_specs:
- filename: lucent-openapi-original.json
  format: json
  label: Lucent API
  slug: lucent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucent/refs/heads/main/openapi/lucent-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lucent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucent secures its APIs with apiKey, http, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lucent
provider_slug: lucent
scheme_count: 2
schemes:
- description: Public key prefixed with `luc_pk_`. Safe to expose in client-side code. For `navigator.sendBeacon` callers that cannot set headers, the key may also be passed as the `api_key` query parameter.
  in: header
  name: lucentApiKey
  parameter: X-Lucent-Api-Key
  sources:
  - openapi/lucent-openapi-original.json
  type: apiKey
- description: API keys prefixed with `luc_api_` or OAuth access tokens prefixed with `luc_oat_`. Legacy static keys prefixed with `luc_mcp_` continue to work.
  name: lucentBearer
  scheme: bearer
  sources:
  - openapi/lucent-openapi-original.json
  type: http
slug: lucent-authentication
source_filename: lucent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/lucent-openapi-original.json\ndocs: https://docs.lucenthq.com/api-reference/authentication\noauth_docs: https://docs.lucenthq.com/mcp/oauth\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2:\n    profile: OAuth 2.1 (fronts the MCP endpoint; PKCE S256, Dynamic Client Registration, refresh tokens)\n    authorizationUrl: https://app.lucenthq.com/oauth/authorize\n    tokenUrl: https://app.lucenthq.com/api/oauth/token\n    scopes: [read:lucent, write:issues]\n    metadata:\n    - well-known/lucent-oauth-authorization-server.json\n    - well-known/lucent-oauth-protected-resource.json\n  token_prefixes:\n    luc_pk_: Ingest public key (write-only; X-Lucent-Api-Key header or api_key query)\n    luc_api_: Data API key (bearer)\n    luc_oat_: OAuth access token (bearer, 1h TTL)\n    luc_mcp_: Legacy static MCP bearer token\nschemes:\n- name: lucentApiKey\n  type: apiKey\n  in:\
  \ header\n  parameter: X-Lucent-Api-Key\n  description: Public key prefixed with `luc_pk_`. Safe to expose in client-side code. For `navigator.sendBeacon`\n    callers that cannot set headers, the key may also be passed as the `api_key` query parameter.\n  sources:\n  - openapi/lucent-openapi-original.json\n- name: lucentBearer\n  type: http\n  scheme: bearer\n  description: API keys prefixed with `luc_api_` or OAuth access tokens prefixed with `luc_oat_`.\n    Legacy static keys prefixed with `luc_mcp_` continue to work.\n  sources:\n  - openapi/lucent-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucent/refs/heads/main/authentication/lucent-authentication.yml
summary_line: apiKey/http/oauth2 · 2 schemes
tags:
- Company
- Session Replay
- Product Analytics
- Bug Detection
- Observability
- Artificial Intelligence
- Developer Tools
- MCP
- Webhooks
---
