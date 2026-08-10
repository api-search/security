---
api_key_in:
- header
api_specs:
- filename: apievangelist-v1-openapi.yml
  format: yaml
  label: API Evangelist Network API
  slug: api-evangelist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist/refs/heads/main/openapi/apievangelist-v1-openapi.yml
- filename: apievangelist-governance-openapi.json
  format: json
  label: API Evangelist Governance & Discovery API
  slug: api-evangelist-governance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist/refs/heads/main/openapi/apievangelist-governance-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Api Evangelist Authentication
name_suffix: Authentication
oauth_flows: []
overview: API Evangelist secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: API Evangelist
provider_slug: api-evangelist
scheme_count: 1
schemes:
- aliases:
  - name: ApiKeyAuth
    note: The network API names the identical x-api-key header scheme ApiKeyAuth; the governance API names it ApiKey. Same header, same location, two names across one base URL.
    spec: openapi/apievangelist-v1-openapi.yml
  description: A Pro or Team key from sign-in. Omit for keyless free-tier access.
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/apievangelist-governance-openapi.json
  - openapi/apievangelist-v1-openapi.yml
  type: apiKey
slug: api-evangelist-authentication
source_filename: api-evangelist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nsource: openapi/apievangelist-governance-openapi.json, openapi/apievangelist-v1-openapi.yml\ndocs: https://developer.apievangelist.com/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  anonymous_supported: true\n  oauth2_flows: []\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: A Pro or Team key from sign-in. Omit for keyless free-tier access.\n  sources:\n  - openapi/apievangelist-governance-openapi.json\n  - openapi/apievangelist-v1-openapi.yml\n  aliases:\n  - name: ApiKeyAuth\n    spec: openapi/apievangelist-v1-openapi.yml\n    note: >-\n      The network API names the identical x-api-key header scheme ApiKeyAuth; the governance API\n      names it ApiKey. Same header, same location, two names across one base URL.\nanonymous_access:\n  supported: true\n  declared: >-\n    both specs declare `security: [{}, {ApiKey: []}]` — the empty requirement is the\n\
  \    machine-readable statement that the API works with no credential\n  tier: free — 5 requests/second, 1,000 requests/day, no signup\n  verified: GET https://api.apievangelist.com/v1/posts?limit=1 returned 200 with no credential\nkey_acquisition:\n  signup: https://api.apievangelist.com/v1/auth/login\n  plans: https://developer.apievangelist.com/plans/\n  contact: info@apievangelist.com\n  note: >-\n    GET /v1/auth/login (200) is the sign-in entry point; POST /v1/billing/checkout starts a paid\n    plan. Neither operation carries an operationId in the governance contract.\ntiering:\n  free: keyless — browse, search and read summaries across the whole network\n  pro: x-api-key — full content (include=content), /guide, /stats, and the artifact-generating\n    governance capabilities\n  enforcement:\n    network_api: 403 {\"error\":\"upgrade_required\",\"tier\":\"pro\"}\n    governance_api: 402 {\"error\":\"payment_required\"}\nmcp:\n  url: https://mcp.apievangelist.com/mcp\n  authentication:\
  \ none\n  note: >-\n    The MCP server card declares authentication type \"none\" and anonymous tools/list returns 200\n    with all 57 tools. Pro tools upsell rather than reject at listing time.\ntransport_security: security/api-evangelist-domain-security.yml\ngaps:\n- No OAuth 2.0 and no OIDC — /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration both 404, so there is no scope surface and no scopes/ artifact.\n- The same header scheme carries two different names across the two contracts.\n- No documented key rotation or revocation procedure.\nx-evidence:\n  checked: '2026-08-10'\n  requests:\n  - {url: 'https://api.apievangelist.com/v1/posts?limit=1', status: 200}\n  - {url: 'https://api.apievangelist.com/v1/auth/login', status: 200}\n  - {url: 'https://developer.apievangelist.com/authentication', status: 200}\n  - {url: 'https://apievangelist.com/.well-known/openid-configuration', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist/refs/heads/main/authentication/api-evangelist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- APIs
- API Evangelist
- Developer Portal
- API Research
- API Governance
- API Discovery
- MCP
- Agents
- API Standards
- API Vocabulary
---
