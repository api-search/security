---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Cerenovus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cerenovus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cerenovus
provider_slug: cerenovus
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://api.cerenovus.ai/authorize
    flow: authorizationCode
    refreshUrl: https://api.cerenovus.ai/token
    scope_count: 9
    tokenUrl: https://api.cerenovus.ai/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://api.cerenovus.ai/
  name: CerenovusOAuth
  registration_endpoint: https://api.cerenovus.ai/register
  response_types_supported:
  - code
  revocation_endpoint: https://api.cerenovus.ai/revoke
  source: https://api.cerenovus.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
slug: cerenovus-authentication
source_filename: cerenovus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.cerenovus.ai/.well-known/oauth-authorization-server\nnote: >-\n  Derived entirely from the provider's own anonymous OAuth discovery documents on\n  api.cerenovus.ai, not from documentation — Cerenovus publishes no developer docs or\n  auth page. There is no OpenAPI to derive securitySchemes from; this profile\n  describes the only authenticated surface found, the OAuth 2.1 authorization server\n  guarding the MCP endpoint at https://api.cerenovus.ai/mcp.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  dynamic_client_registration: true\nschemes:\n- name: CerenovusOAuth\n  type: oauth2\n  source: https://api.cerenovus.ai/.well-known/oauth-authorization-server\n  issuer: https://api.cerenovus.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cerenovus.ai/authorize\n    tokenUrl: https://api.cerenovus.ai/token\n    refreshUrl: https://api.cerenovus.ai/token\n\
  \    scope_count: 9\n  revocation_endpoint: https://api.cerenovus.ai/revoke\n  registration_endpoint: https://api.cerenovus.ai/register\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\nprotected_resources:\n- resource: https://api.cerenovus.ai/\n  resource_name: Compendium vault\n  authorization_servers:\n  - https://api.cerenovus.ai/\n  metadata: https://api.cerenovus.ai/.well-known/oauth-protected-resource\nchallenge:\n  status: 401\n  header: WWW-Authenticate\n  scheme: Bearer\n  carries_resource_metadata: true\n  example: >-\n    Bearer error=\"invalid_token\", error_description=\"Missing Authorization header\",\n    resource_metadata=\"https://api.cerenovus.ai/.well-known/oauth-protected-resource\"\nx-evidence:\n  fetched: '2026-08-14'\n  probes:\n  - url: https://api.cerenovus.ai/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n  - url: https://api.cerenovus.ai/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://api.cerenovus.ai/authorize\n    http_status: 400\n    note: rejects a request with no client_id, confirming a live authorization endpoint\n  - url: https://api.cerenovus.ai/token\n    http_status: 405\n    note: GET rejected; POST-only token endpoint\n  - url: https://api.cerenovus.ai/register\n    http_status: 405\n    note: GET rejected; POST-only dynamic client registration endpoint\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerenovus/refs/heads/main/authentication/cerenovus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Enterprise Software
- Decision Intelligence
- Knowledge Management
- Private Equity
- Due Diligence
- Model Context Protocol
- Y Combinator
---
