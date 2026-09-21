---
anonymous_access: true
api_key_in: []
api_specs:
- filename: movehome-org-raia-portal-feed-openapi.yaml
  format: yaml
  label: RAIA Portal Feed API (MoveHome.org implementation)
  slug: raia-portal-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/openapi/movehome-org-raia-portal-feed-openapi.yaml
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Movehome Org Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Move Home Organisation CIC secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Move Home Organisation CIC
provider_slug: movehome-org
scheme_count: 2
schemes:
- controls:
  - per-IP rate limits (60/min agent surfaces; 5/min enquiry; 10/min registry register; 5/min flag)
  - create_enquiry duplicate suppression (same email + listing within ~10 min) and a per-email hourly cap
  - registry registration validates the submitted card by fetching it from the declared well-known URI
  name: Anonymous
  note: The agent card declares no securitySchemes, which is accurate. CORS is open on every anonymous surface, so browser-hosted agents can call them directly.
  observed:
  - POST /api/a2a message/send with no credentials -> 200 completed Task (2026-09-19)
  - POST /mcp tools/list with no credentials -> 200, 2 tools
  - POST /api/registry/mcp tools/list with no credentials -> 200, 3 tools
  - GET /api/registry/v1/agents?limit=3 -> 200
  surfaces:
  - https://movehome.org/api/a2a (A2A JSON-RPC — search_properties, get_property, create_enquiry)
  - https://movehome.org/mcp and https://movehome.org/api/mcp (MCP, read-only)
  - https://movehome.org/api/registry/mcp (MCP, read-only)
  - https://movehome.org/api/registry/v1/* (REST — reads AND the register / re-sync / flag writes)
  - https://movehome.org/api/enquire (website enquiry form POST)
  type: none
- client_authentication: HTTP Basic (client_id:client_secret) or form fields client_id / client_secret; grant_type must be client_credentials
  credential_issuance:
    contact: admin@movehome.org
    how: out-of-band by the MoveHome operator (scripts/portal-create-credential.cjs in the provider's repository); the secret is shown once
    signup: none — no self-service developer portal
  description: 'Server-to-server OAuth2 client credentials flow. The token endpoint is

    published by the implementer; credentials are issued out-of-band

    during onboarding. Tokens are short-lived Bearer JWTs.'
  flows:
  - flow: clientCredentials
    scopes: 3
    scopes_list:
    - feed.read
    - feed.write
    - products.write
    tokenUrl: https://movehome.org/oauth/token
    tokenUrl_in_spec: https://feed.example.com/oauth/token
  name: OAuth2ClientCredentials
  observed:
  - 'POST /oauth/token grant_type=client_credentials (no client) -> 401 application/problem+json {"type":"https://movehome.org/errors/unauthorized","detail":"Missing client_id / client_secret. Use HTTP Basic or form fields.","instance":"/oauth/token"} with WWW-Authenticate: Bearer realm="raia-portal-feed"'
  - 'GET /api/raia/portal/v1/listings/AE-PROBE (no token) -> 401 {"detail":"Missing Authorization: Bearer header."}'
  - GET /api/raia/portal/v1/branches/x/listings (no token) -> 401
  - 'GET /api/raia/portal/v1/healthz -> 200 (security: [])'
  rate_limit: token endpoint 10 requests/min per client; API 60/min per credential per endpoint group
  sources:
  - openapi/movehome-org-raia-portal-feed-openapi.yaml
  - https://github.com/MoveHome/MoveHome.Org/blob/main/docs/raia-portal-feed-api.md#3-authentication
  - https://github.com/MoveHome/MoveHome.Org/blob/main/src/app/oauth/token/route.ts
  surfaces:
  - https://movehome.org/api/raia/portal/v1/* (every operation except GET /healthz)
  token:
    alg: HS256
    format: JWT
    header: 'Authorization: Bearer <access_token>'
    response: '{ access_token, token_type: "Bearer", expires_in: 3600, scope }'
    scope_handling: requested scope is intersected with the credential's allowed_scopes; omit scope to receive all allowed scopes
    ttl_seconds: 3600
    verification: server-side only — HS256 with a shared secret; the published JWKS (/.well-known/jwks.json) is empty, so third parties cannot verify these tokens (the RAIA spec recommends RS256 for that reason)
  type: oauth2
slug: movehome-org-authentication
source_filename: movehome-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/movehome-org-raia-portal-feed-openapi.yaml\ndocs:\n- https://movehome.org/skills.md\n- https://github.com/MoveHome/MoveHome.Org/blob/main/docs/raia-portal-feed-api.md#3-authentication\n- https://github.com/MoveHome/MoveHome.Org/blob/main/docs/raia-a2a-api.md\nsummary:\n  types:\n  - none\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  bearer: true\n  credential_classes: 2\n  headline: >-\n    Two postures on one host. The agent-facing surfaces — the A2A agent (all three skills, including the\n    create_enquiry write), both MCP servers and the A2A-registry REST API — are ANONYMOUS: no key, no token,\n    no signup (\"Auth: none (anonymous)\", skills.md), with per-IP rate limits as the only gate. The inbound\n    RAIA Portal Feed API is OAuth 2.0 client credentials: the MoveHome operator issues a client_id and\n    client_secret out-of-band, bound to one agent, a default branch and an allowed\
  \ scope set; POST\n    https://movehome.org/oauth/token (HTTP Basic or form fields) mints a 1-hour HS256 Bearer JWT scoped to\n    feed.read / feed.write / products.write. No OIDC, no API keys, no RFC 8414/9728 discovery documents.\nschemes:\n- name: Anonymous\n  type: none\n  surfaces:\n  - https://movehome.org/api/a2a (A2A JSON-RPC — search_properties, get_property, create_enquiry)\n  - https://movehome.org/mcp and https://movehome.org/api/mcp (MCP, read-only)\n  - https://movehome.org/api/registry/mcp (MCP, read-only)\n  - https://movehome.org/api/registry/v1/* (REST — reads AND the register / re-sync / flag writes)\n  - https://movehome.org/api/enquire (website enquiry form POST)\n  controls:\n  - per-IP rate limits (60/min agent surfaces; 5/min enquiry; 10/min registry register; 5/min flag)\n  - create_enquiry duplicate suppression (same email + listing within ~10 min) and a per-email hourly cap\n  - registry registration validates the submitted card by fetching it from the declared\
  \ well-known URI\n  observed:\n  - 'POST /api/a2a message/send with no credentials -> 200 completed Task (2026-09-19)'\n  - 'POST /mcp tools/list with no credentials -> 200, 2 tools'\n  - 'POST /api/registry/mcp tools/list with no credentials -> 200, 3 tools'\n  - 'GET /api/registry/v1/agents?limit=3 -> 200'\n  note: >-\n    The agent card declares no securitySchemes, which is accurate. CORS is open on every anonymous surface,\n    so browser-hosted agents can call them directly.\n- name: OAuth2ClientCredentials\n  type: oauth2\n  surfaces:\n  - https://movehome.org/api/raia/portal/v1/* (every operation except GET /healthz)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://movehome.org/oauth/token\n    tokenUrl_in_spec: https://feed.example.com/oauth/token\n    scopes: 3\n    scopes_list: [feed.read, feed.write, products.write]\n  client_authentication: HTTP Basic (client_id:client_secret) or form fields client_id / client_secret; grant_type must be client_credentials\n  token:\n\
  \    format: JWT\n    alg: HS256\n    ttl_seconds: 3600\n    header: 'Authorization: Bearer <access_token>'\n    response: '{ access_token, token_type: \"Bearer\", expires_in: 3600, scope }'\n    scope_handling: requested scope is intersected with the credential's allowed_scopes; omit scope to receive all allowed scopes\n    verification: server-side only — HS256 with a shared secret; the published JWKS (/.well-known/jwks.json) is empty, so third parties cannot verify these tokens (the RAIA spec recommends RS256 for that reason)\n  credential_issuance:\n    how: out-of-band by the MoveHome operator (scripts/portal-create-credential.cjs in the provider's repository); the secret is shown once\n    contact: admin@movehome.org\n    signup: none — no self-service developer portal\n  rate_limit: token endpoint 10 requests/min per client; API 60/min per credential per endpoint group\n  observed:\n  - 'POST /oauth/token grant_type=client_credentials (no client) -> 401 application/problem+json\
  \ {\"type\":\"https://movehome.org/errors/unauthorized\",\"detail\":\"Missing client_id / client_secret. Use HTTP Basic or form fields.\",\"instance\":\"/oauth/token\"} with WWW-Authenticate: Bearer realm=\"raia-portal-feed\"'\n  - 'GET /api/raia/portal/v1/listings/AE-PROBE (no token) -> 401 {\"detail\":\"Missing Authorization: Bearer header.\"}'\n  - 'GET /api/raia/portal/v1/branches/x/listings (no token) -> 401'\n  - 'GET /api/raia/portal/v1/healthz -> 200 (security: [])'\n  description: |-\n    Server-to-server OAuth2 client credentials flow. The token endpoint is\n    published by the implementer; credentials are issued out-of-band\n    during onboarding. Tokens are short-lived Bearer JWTs.\n  sources:\n  - openapi/movehome-org-raia-portal-feed-openapi.yaml\n  - https://github.com/MoveHome/MoveHome.Org/blob/main/docs/raia-portal-feed-api.md#3-authentication\n  - https://github.com/MoveHome/MoveHome.Org/blob/main/src/app/oauth/token/route.ts\ndiscovery:\n  openid_configuration: {url:\
  \ 'https://movehome.org/.well-known/openid-configuration', status: 404}\n  oauth_authorization_server: {url: 'https://movehome.org/.well-known/oauth-authorization-server', status: 404}\n  oauth_protected_resource: {url: 'https://movehome.org/.well-known/oauth-protected-resource', status: 404}\n  jwks: {url: 'https://movehome.org/.well-known/jwks.json', status: 200, body: '{\"keys\":[]}'}\nscopes_detail: scopes/movehome-org-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/authentication/movehome-org-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Real-Estate
- Property
- Lettings
- Property Sales
- Agents
- A2A
- MCP
- agent-native
- Agent Registry
- Non-Profit
- Open-Source
- RAIA Protocol
- United Kingdom
---
