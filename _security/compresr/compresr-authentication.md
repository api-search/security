---
api_key_in:
- header
api_specs:
- filename: compresr-openapi-original.json
  format: json
  label: Compresr Platform API
  slug: compresr-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/compresr/refs/heads/main/openapi/compresr-openapi-original.json
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Compresr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Compresr secures its APIs with apiKey, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Compresr
provider_slug: compresr
scheme_count: 3
schemes:
- docs: https://compresr.ai/docs/authentication
  in: header
  key_prefix: cmp_
  name: X-API-Key
  parameter_name: X-API-Key
  scopes:
  - demo
  - user
  - enterprise
  sources:
  - openapi/compresr-openapi-original.json
  - https://compresr.ai/docs/authentication
  type: apiKey
- flows:
  - authorizationUrl: https://api.compresr.ai/oauth/authorize
    flow: authorizationCode
    pkce: true
    refresh: true
    tokenUrl: https://api.compresr.ai/oauth/token
  - deviceAuthorizationUrl: https://api.compresr.ai/oauth/device_authorization
    flow: deviceCode
    tokenUrl: https://api.compresr.ai/oauth/token
  name: OAuth2
  purpose: CLI and dashboard login (not per-request API authentication)
  sources:
  - openapi/compresr-openapi-original.json
  type: oauth2
- name: HTTPBearer
  note: declared in OpenAPI securitySchemes (FastAPI-generated); actual request auth is X-API-Key
  scheme: bearer
  sources:
  - openapi/compresr-openapi-original.json
  type: http
slug: compresr-authentication
source_filename: compresr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/compresr-openapi-original.json\ndocs: https://compresr.ai/docs/authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - http\n  api_key_in:\n  - header\n  api_key_header: X-API-Key\n  api_key_prefix: cmp_\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\n  pkce: true\nnotes: >-\n  The public API authenticates with an X-API-Key header carrying a cmp_-prefixed key\n  issued from the dashboard (documented at /docs/authentication). The OpenAPI's\n  generated securitySchemes only declares an HTTPBearer http/bearer scheme; the\n  operations themselves take X-API-Key as a header parameter. A separate OAuth 2.0\n  authorization server (authorization-code with PKCE, device-code, and refresh-token\n  grants) backs CLI (`compresr-sdk login`) and dashboard sign-in, not per-request API\n  auth. API keys carry a scope of demo | user | enterprise.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter_name:\
  \ X-API-Key\n  key_prefix: cmp_\n  scopes:\n  - demo\n  - user\n  - enterprise\n  docs: https://compresr.ai/docs/authentication\n  sources:\n  - openapi/compresr-openapi-original.json\n  - https://compresr.ai/docs/authentication\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.compresr.ai/oauth/authorize\n    tokenUrl: https://api.compresr.ai/oauth/token\n    pkce: true\n    refresh: true\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://api.compresr.ai/oauth/device_authorization\n    tokenUrl: https://api.compresr.ai/oauth/token\n  purpose: CLI and dashboard login (not per-request API authentication)\n  sources:\n  - openapi/compresr-openapi-original.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  note: declared in OpenAPI securitySchemes (FastAPI-generated); actual request auth is X-API-Key\n  sources:\n  - openapi/compresr-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compresr/refs/heads/main/authentication/compresr-authentication.yml
summary_line: apiKey/oauth2/http · 3 schemes
tags:
- LLM
- Context Compression
- Prompt Engineering
- RAG
- AI Infrastructure
- Developer Tools
- Agents
- Tokens
- API
- Y Combinator
---
