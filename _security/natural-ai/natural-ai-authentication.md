---
api_key_in: []
api_specs:
- filename: natural-ai-openapi-original.json
  format: json
  label: Natural API
  slug: natural-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Natural Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Natural AI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Natural AI
provider_slug: natural-ai
scheme_count: 2
schemes:
- description: 'Bearer authentication. Send an API key, agent key, or OAuth access token as Authorization: Bearer <credential>.'
  name: HTTPBearer
  scheme: bearer
  source: openapi/natural-ai-openapi-original.json
  type: http
- flows:
  - authorizationUrl: https://api.natural.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.natural.com/oauth/register
    revocationUrl: https://api.natural.com/oauth/revoke
    tokenUrl: https://api.natural.com/oauth/token
    token_endpoint_auth: none
  name: OAuth2
  source: https://api.natural.com/.well-known/oauth-authorization-server
  type: oauth2
slug: natural-ai-authentication
source_filename: natural-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.natural.com/api-reference/authentication\ndocs: https://docs.natural.com/api-reference/authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  credential_modes: [api-key, agent-key, user-scoped-oauth, agent-scoped-oauth]\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  source: openapi/natural-ai-openapi-original.json\n  description: >-\n    Bearer authentication. Send an API key, agent key, or OAuth access token as\n    Authorization: Bearer <credential>.\n- name: OAuth2\n  type: oauth2\n  source: https://api.natural.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.natural.com/oauth/authorize\n    tokenUrl: https://api.natural.com/oauth/token\n    registrationUrl: https://api.natural.com/oauth/register\n    revocationUrl: https://api.natural.com/oauth/revoke\n    pkce:\
  \ S256\n    token_endpoint_auth: none\ncredential_modes:\n- mode: api-key\n  prefix: sk_ntl_\n  format: sk_ntl_{environment}_{secret}\n  environments: [prod]\n  acts_as: your party\n  scopable: true\n- mode: agent-key\n  prefix: ak_ntl_\n  format: ak_ntl_{environment}_{secret}\n  acts_as: one specific bound agent, verified by the credential\n- mode: user-scoped-oauth\n  flow: browser OAuth consent\n  acts_as: the authorizing user/party\n- mode: agent-scoped-oauth\n  flow: browser OAuth consent\n  acts_as: a selected or new agent, verified\nnotes:\n- Credentials are scoped and can never exceed the issuing party's permissions.\n- Keys are high-entropy, shown once, stored only as one-way hashes.\n- OAuth uses 2.1 with PKCE and short-lived access tokens; access tokens signed by AWS KMS.\n- Agent-attributed money movement requires an X-Instance-ID header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/authentication/natural-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai
- Payments
- Agents
- Fintech
- Money Movement
- Wallets
- Agentic Payments
- MCP
---
