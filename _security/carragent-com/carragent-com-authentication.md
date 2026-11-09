---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carragent-com-agents-api-openapi.yml
  format: yaml
  label: carragent-com Agents API
  slug: carragent-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carragent-com/openapi/carragent-com-agents-api-openapi.yml
auth_types: []
description: Carragent API can be accessed without authentication, but optionally OAuth 2.0 tokens can be obtained via client credentials or JWT‑bearer grant to raise the rate limit.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Carragent Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: carragent-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: carragent-com
provider_slug: carragent-com
scheme_count: 2
schemes:
- evidence: 'OAuth 2.0 client credentials (RFC 6749, section 4.4): a client you register once and keep. Its secret does not expire; its tokens last 1 hour.'
  flows:
  - client_credentials
  how_to_obtain: Register a client via POST https://carragent.com/api/oauth2/register, then request a token with grant_type=client_credentials using HTTP Basic authentication (client_id and client_secret) or form fields.
  name: OAuth 2.0 client credentials
  scopes:
  - agents:read
  - plans:read
  - search:read
  token_url: https://carragent.com/api/oauth2/token
  type: oauth2
- evidence: 'Anonymous agent registration (`anonymous`): the agent registers itself and keeps no client or secret. It holds an identity assertion for 24 hours and exchanges it for tokens (RFC 7523, the JWT-bearer grant).'
  flows:
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  how_to_obtain: 'POST https://carragent.com/agent/identity with body {"type": "anonymous"} to receive an identity_assertion JWT, then POST https://carragent.com/api/oauth2/token with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer and assertion=<identity_assertion>.'
  name: OAuth 2.0 JWT‑bearer grant (anonymous agent registration)
  scopes:
  - agents:read
  - plans:read
  - search:read
  token_url: https://carragent.com/api/oauth2/token
  type: oauth2
slug: carragent-com-authentication
source_filename: carragent-com-authentication.yml
source_heading: Authentication Profile
source_url: https://carragent.com/auth.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://carragent.com/auth.md\nsources:\n- https://carragent.com/auth.md\ndescription: Carragent API can be accessed without authentication, but optionally OAuth 2.0 tokens can be obtained via client credentials or JWT‑bearer\n  grant to raise the rate limit.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 client credentials\n  evidence: 'OAuth 2.0 client credentials (RFC 6749, section 4.4): a client you register once and keep. Its secret does not expire; its tokens\n    last 1 hour.'\n  flows:\n  - client_credentials\n  token_url: https://carragent.com/api/oauth2/token\n  scopes:\n  - agents:read\n  - plans:read\n  - search:read\n  how_to_obtain: Register a client via POST https://carragent.com/api/oauth2/register, then request a token with grant_type=client_credentials\n    using HTTP Basic authentication (client_id and client_secret) or form fields.\n- type: oauth2\n  name: OAuth\
  \ 2.0 JWT‑bearer grant (anonymous agent registration)\n  evidence: 'Anonymous agent registration (`anonymous`): the agent registers itself and keeps no client or secret. It holds an identity assertion\n    for 24 hours and exchanges it for tokens (RFC 7523, the JWT-bearer grant).'\n  flows:\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_url: https://carragent.com/api/oauth2/token\n  scopes:\n  - agents:read\n  - plans:read\n  - search:read\n  how_to_obtain: 'POST https://carragent.com/agent/identity with body {\"type\": \"anonymous\"} to receive an identity_assertion JWT, then POST https://carragent.com/api/oauth2/token\n    with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer and assertion=<identity_assertion>.'\nnote: Requests without an Authorization header are allowed (public read‑only access) with a limit of 60 requests per minute per IP.\ndocs: https://carragent.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/carragent-com/authentication/carragent-com-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Business tools integration
---
