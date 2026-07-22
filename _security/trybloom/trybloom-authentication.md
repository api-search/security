---
api_key_in:
- header
api_specs:
- filename: trybloom-api-openapi.json
  format: json
  label: Bloom API
  slug: bloom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/openapi/trybloom-api-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Trybloom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Bloom secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Bloom
provider_slug: trybloom
scheme_count: 3
schemes:
- description: 'Bloom API key, for example `x-api-key: bloom_sk_...`.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/trybloom-api-openapi.json
  type: apiKey
- description: Bloom API key (`Bearer bloom_sk_...`) or Bloom OAuth access token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/trybloom-api-openapi.json
  type: http
- description: App-integration OAuth (not declared in the OpenAPI securitySchemes; documented in docs/api/authentication with RFC 8414 metadata at /.well-known/oauth-authorization-server).
  flows:
  - authorizationUrl: https://www.trybloom.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token
  issuer: https://www.trybloom.ai/api/auth
  name: Bloom OAuth
  registration: https://www.trybloom.ai/api/auth/oauth2/register
  scopes: scopes/trybloom-scopes.yml
  sources:
  - https://www.trybloom.ai/docs/api/authentication
  - well-known/trybloom-oauth-authorization-server.json
  type: oauth2
slug: trybloom-authentication
source_filename: trybloom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/trybloom-api-openapi.json\ndocs: https://www.trybloom.ai/docs/api/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\nnotes: >-\n  Every request needs a Bloom API key (bloom_sk_...) or a Bloom OAuth access\n  token. The key is accepted in either header; x-api-key wins when both are\n  present. OAuth tokens resolve to the same user identity as an API key (same\n  access to brands, images, credits, plan gates, workspaces). Public clients\n  use Authorization Code + PKCE S256 with dynamic client registration and no\n  client_secret; wildcard redirect URIs are not supported. Keys are generated\n  at https://www.trybloom.ai/settings#api-keys.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Bloom API key, for example `x-api-key: bloom_sk_...`.'\n  sources:\n\
  \  - openapi/trybloom-api-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Bloom API key (`Bearer bloom_sk_...`) or Bloom OAuth access token.\n  sources:\n  - openapi/trybloom-api-openapi.json\n- name: Bloom OAuth\n  type: oauth2\n  description: >-\n    App-integration OAuth (not declared in the OpenAPI securitySchemes;\n    documented in docs/api/authentication with RFC 8414 metadata at\n    /.well-known/oauth-authorization-server).\n  issuer: https://www.trybloom.ai/api/auth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.trybloom.ai/api/auth/oauth2/authorize\n    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token\n  registration: https://www.trybloom.ai/api/auth/oauth2/register\n  scopes: scopes/trybloom-scopes.yml\n  sources:\n  - https://www.trybloom.ai/docs/api/authentication\n\
  \  - well-known/trybloom-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/authentication/trybloom-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Brand Management
- Image Generation
- Artificial Intelligence
- Agents
- MCP
- Marketing
- Creative
---
