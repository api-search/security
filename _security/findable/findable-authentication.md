---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Findable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Findable secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Findable
provider_slug: findable
scheme_count: 3
schemes:
- description: Organization-scoped API key required on all Partner API requests. Keys are provisioned by a Findable representative and are prefixed fk_live_ (production) or fk_test_ (sandbox). Determines which building owners are accessible. 401 = missing/invalid key; 403 = key lacks access to resource.
  in: header
  name: apiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://docs.findable.ai/api/authentication
  type: apiKey
- bearerFormat: session-token
  description: 'Short-lived session token for client-side access, minted server-side via POST https://api.findable.ai/v1/building_owners/{OWNER_ID}/sessions (body {"expires_in": <seconds>}). Scoped to a single building owner; default TTL 1 hour, maximum 24 hours. Sent as Authorization: Bearer [example key]'
  name: sessionBearer
  scheme: bearer
  sources:
  - https://docs.findable.ai/api/authentication
  token_prefix: ft_
  type: http
- flows:
  - description: OAuth 2.1 with PKCE used by the hosted Findable MCP server (https://mcp.findable.ai). Access is tied to the individual Findable user account; every tool call is checked against the same permissions as the Findable app.
    flow: authorizationCode
    pkce: true
  name: mcpOAuth
  sources:
  - https://docs.findable.ai/mcp
  type: oauth2
slug: findable-authentication
source_filename: findable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.findable.ai/api/authentication\ndocs: https://docs.findable.ai/api/authentication\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  api_key_header: x-api-key\n  bearer_token_prefix: ft_\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Findable Partner API authenticates with a static organization-scoped API\n    key sent in the x-api-key header. For browser/client-side use, a server\n    exchanges its API key for a short-lived building-owner-scoped session token\n    (Bearer [example key]). The hosted MCP server (mcp.findable.ai) authenticates end\n    users with OAuth 2.1 + PKCE tied to their Findable account.\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    description: >-\n      Organization-scoped API key required on all Partner API requests. Keys are\n      provisioned by a Findable representative and are prefixed fk_live_\n\
  \      (production) or fk_test_ (sandbox). Determines which building owners are\n      accessible. 401 = missing/invalid key; 403 = key lacks access to resource.\n    sources: [https://docs.findable.ai/api/authentication]\n  - name: sessionBearer\n    type: http\n    scheme: bearer\n    bearerFormat: session-token\n    token_prefix: ft_\n    description: >-\n      Short-lived session token for client-side access, minted server-side via\n      POST https://api.findable.ai/v1/building_owners/{OWNER_ID}/sessions (body\n      {\"expires_in\": <seconds>}). Scoped to a single building owner; default TTL\n      1 hour, maximum 24 hours. Sent as Authorization: Bearer [example key]\n    sources: [https://docs.findable.ai/api/authentication]\n  - name: mcpOAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        pkce: true\n        description: >-\n          OAuth 2.1 with PKCE used by the hosted Findable MCP server\n          (https://mcp.findable.ai). Access is tied to the\
  \ individual Findable\n          user account; every tool call is checked against the same permissions\n          as the Findable app.\n    sources: [https://docs.findable.ai/mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findable/refs/heads/main/authentication/findable-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Building Intelligence
- Property Technology
- PropTech
- Facilities Management
- Building Documentation
- Compliance
- Artificial Intelligence
- Document Search
- Construction
---
