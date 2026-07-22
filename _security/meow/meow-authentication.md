---
api_key_in:
- header
api_specs:
- filename: meow-openapi.yaml
  format: yaml
  label: Meow API
  slug: meow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meow/refs/heads/main/openapi/meow-openapi.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Meow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Meow secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Meow
provider_slug: meow
scheme_count: 3
schemes:
- description: Your Meow API key, sent in the `x-api-key` header for authentication.
  docs: https://developer.meow.com/authentication
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/meow-openapi.yaml
  type: apiKey
- description: Optional header to scope a multi-entity API key to a specific business entity (UUID). Not a standalone credential; used alongside x-api-key.
  in: header
  name: entityScope
  parameter: x-entity-id
  sources:
  - openapi/meow-openapi.yaml
  type: apiKey
- description: OAuth 2.1 with PKCE for the Meow MCP server. meow.read is always granted; meow.transfers, meow.cards, and meow.billing are opt-in via a post-login scope picker gated by the user's role.
  flow: authorizationCode
  name: mcpOAuth
  pkce: true
  scopes:
  - meow.read
  - meow.transfers
  - meow.cards
  - meow.billing
  server: https://mcp.meow.com
  sources:
  - https://developer.meow.com/mcp/authentication
  type: oauth2
slug: meow-authentication
source_filename: meow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/meow-openapi.yaml\ndocs: https://developer.meow.com/authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nnotes: >-\n  The REST API authenticates with an API key in the x-api-key header. Keys are\n  created and scoped from the Meow dashboard and carry granular scopes (see\n  scopes/meow-scopes.yml). For API keys with access to multiple entities, the\n  optional x-entity-id header scopes a request to a specific entity; list\n  accessible entities with GET /api-keys/accessible-entities. The Meow MCP\n  server adds a second, OAuth 2.1-with-PKCE surface for AI assistants at\n  https://mcp.meow.com (plus an API-key/bearer CLI surface at\n  https://mcp.meow.com/cli); it acts as an authorization proxy in front of\n  Meow's identity provider with a post-login scope picker over meow.* scopes.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n\
  \  parameter: x-api-key\n  description: Your Meow API key, sent in the `x-api-key` header for authentication.\n  sources:\n  - openapi/meow-openapi.yaml\n  docs: https://developer.meow.com/authentication\n- name: entityScope\n  type: apiKey\n  in: header\n  parameter: x-entity-id\n  description: >-\n    Optional header to scope a multi-entity API key to a specific business\n    entity (UUID). Not a standalone credential; used alongside x-api-key.\n  sources:\n  - openapi/meow-openapi.yaml\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  server: https://mcp.meow.com\n  description: >-\n    OAuth 2.1 with PKCE for the Meow MCP server. meow.read is always granted;\n    meow.transfers, meow.cards, and meow.billing are opt-in via a post-login\n    scope picker gated by the user's role.\n  scopes:\n  - meow.read\n  - meow.transfers\n  - meow.cards\n  - meow.billing\n  sources:\n  - https://developer.meow.com/mcp/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meow/refs/heads/main/authentication/meow-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Banking
- Fintech
- Business Banking
- Payments
- Cards
- Invoicing
- Treasury
- Cryptocurrency
- Webhooks
- MCP
- API
---
