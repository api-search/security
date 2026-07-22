---
api_key_in:
- header
api_specs:
- filename: sourcebot-public-openapi-original.json
  format: json
  label: Sourcebot Public API
  slug: sourcebot-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcebot/refs/heads/main/openapi/sourcebot-public-openapi-original.json
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sourcebot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sourcebot secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sourcebot
provider_slug: sourcebot
scheme_count: 3
schemes:
- description: Bearer authentication header of the form `Bearer <token>`, where <token> is your Sourcebot API key. Standard integration mechanism for the public REST API.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/sourcebot-public-openapi-original.json
  type: http
- description: 'Header of the form `X-Sourcebot-Api-Key: <token>`, where <token> is your API key.'
  in: header
  name: apiKeyHeader
  parameter_name: X-Sourcebot-Api-Key
  sources:
  - openapi/sourcebot-public-openapi-original.json
  type: apiKey
- authorization_url: https://app.sourcebot.dev/oauth/authorize
  description: Enterprise (EE) OAuth 2.0 flow used to authenticate MCP / agent clients against the hosted instance. Advertised via RFC 8414 authorization-server metadata with DPoP (ES256) and PKCE (S256); supports dynamic client registration.
  flow: authorizationCode
  name: oauth2-ee
  registration_url: https://app.sourcebot.dev/api/ee/oauth/register
  revocation_url: https://app.sourcebot.dev/api/ee/oauth/revoke
  sources:
  - well-known/sourcebot-oauth-authorization-server.json
  token_url: https://app.sourcebot.dev/api/ee/oauth/token
  type: oauth2
slug: sourcebot-authentication
source_filename: sourcebot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sourcebot-public-openapi-original.json\ndocs: https://docs.sourcebot.dev/docs/api-reference/authentication\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]     # EE / MCP only, see note\n  anonymous_allowed: true               # some instances permit unauthenticated access\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer authentication header of the form `Bearer <token>`, where <token> is your\n      Sourcebot API key. Standard integration mechanism for the public REST API.\n    sources: [openapi/sourcebot-public-openapi-original.json]\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter_name: X-Sourcebot-Api-Key\n    description: \"Header of the form `X-Sourcebot-Api-Key: <token>`, where <token> is your API key.\"\n    sources: [openapi/sourcebot-public-openapi-original.json]\n\
  \  - name: oauth2-ee\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      Enterprise (EE) OAuth 2.0 flow used to authenticate MCP / agent clients against the\n      hosted instance. Advertised via RFC 8414 authorization-server metadata with DPoP\n      (ES256) and PKCE (S256); supports dynamic client registration.\n    authorization_url: https://app.sourcebot.dev/oauth/authorize\n    token_url: https://app.sourcebot.dev/api/ee/oauth/token\n    registration_url: https://app.sourcebot.dev/api/ee/oauth/register\n    revocation_url: https://app.sourcebot.dev/api/ee/oauth/revoke\n    sources: [well-known/sourcebot-oauth-authorization-server.json]\nnotes: >-\n  API keys are created in the instance Settings UI. EE endpoints (/api/ee/*) additionally\n  require an active Sourcebot license and OWNER role. OAuth bearer tokens are EE-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcebot/refs/heads/main/authentication/sourcebot-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Company
- Code Search
- Code Intelligence
- Developer Tools
- Source Code
- Git
- MCP
- AI Coding Agents
- Enterprise Search
- Self-Hosted
---
