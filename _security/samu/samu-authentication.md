---
api_key_in:
- header
api_specs:
- filename: samu-openapi.yml
  format: yaml
  label: API Samu
  slug: api-samu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Samu Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Samu secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Samu
provider_slug: samu
scheme_count: 2
schemes:
- applies_to: https://api.samu.ai/api/* (all 10 REST operations)
  description: API key de la cuenta
  in: header
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/samu-openapi.yml
  type: apiKey
- applies_to: https://api.samu.ai/mcp
  authorizationUrl: https://api.samu.ai/oauth/authorize
  bearer_methods:
  - header
  code_challenge_methods:
  - S256
  flows:
  - authorizationCode
  - refreshToken
  issuer: https://api.samu.ai
  name: MCP OAuth 2.1
  registrationUrl: https://api.samu.ai/oauth/register
  revocationUrl: https://api.samu.ai/oauth/revoke
  scopes:
  - mcp:read
  sources:
  - well-known/samu-oauth-authorization-server.json
  - well-known/samu-oauth-protected-resource-mcp.json
  tokenUrl: https://api.samu.ai/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: samu-authentication
source_filename: samu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/samu-openapi.yml\ndocs: https://api.samu.ai/docs\nnote: >-\n  Two distinct auth models on one host. The REST API (api.samu.ai/api/*) uses a\n  static account API key in a header literally named \"apiKey\" (not Authorization,\n  not X-API-Key) — worth noting because it is unusual and easy to get wrong. The\n  MCP endpoint (api.samu.ai/mcp) uses OAuth 2.1 bearer tokens with dynamic client\n  registration and PKCE, advertised via RFC 8414 metadata; it rejects anonymous\n  calls with 401 MCP_UNAUTHORIZED and a WWW-Authenticate challenge pointing at\n  its RFC 9728 protected-resource metadata. Samu publishes no page describing how\n  to obtain an API key; the pricing page places API access on the Enterprise plan\n  and MCP on the Pro plan, so provisioning is sales-mediated.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\nschemes:\n- name: ApiKeyAuth\n\
  \  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API key de la cuenta\n  applies_to: https://api.samu.ai/api/* (all 10 REST operations)\n  sources:\n  - openapi/samu-openapi.yml\n- name: MCP OAuth 2.1\n  type: oauth2\n  bearer_methods: [header]\n  applies_to: https://api.samu.ai/mcp\n  issuer: https://api.samu.ai\n  authorizationUrl: https://api.samu.ai/oauth/authorize\n  tokenUrl: https://api.samu.ai/oauth/token\n  registrationUrl: https://api.samu.ai/oauth/register\n  revocationUrl: https://api.samu.ai/oauth/revoke\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  scopes: [mcp:read]\n  flows: [authorizationCode, refreshToken]\n  sources:\n  - well-known/samu-oauth-authorization-server.json\n  - well-known/samu-oauth-protected-resource-mcp.json\nprovisioning:\n  self_serve: false\n  note: >-\n    No public sign-up for API credentials. Pricing page sells \"acceso a la API\"\n    (API Out / API In) on Enterprise ($900/mo) and MCP on Pro ($250/mo).\n\
  \  source: https://samu.ai/precios\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/authentication/samu-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Conversation Intelligence
- CRM
- Call Recording
- Analytics
- Latin America
- Transcription
- WhatsApp
- MCP
- Agent Native
---
