---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: compeller-ai-auth-api-openapi.yml
  format: yaml
  label: Compeller Auth API
  slug: compeller-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-auth-api-openapi.yml
- filename: compeller-ai-compels-api-openapi.yml
  format: yaml
  label: Compeller Compels API
  slug: compeller-ai-compels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-compels-api-openapi.yml
- filename: compeller-ai-discovery-api-openapi.yml
  format: yaml
  label: Compeller Discovery API
  slug: compeller-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-discovery-api-openapi.yml
- filename: compeller-ai-lighting-api-openapi.yml
  format: yaml
  label: Compeller Lighting API
  slug: compeller-ai-lighting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-lighting-api-openapi.yml
- filename: compeller-ai-media-api-openapi.yml
  format: yaml
  label: Compeller Media API
  slug: compeller-ai-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-media-api-openapi.yml
- filename: compeller-ai-music-api-openapi.yml
  format: yaml
  label: Compeller Music API
  slug: compeller-ai-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-music-api-openapi.yml
- filename: compeller-ai-renderings-api-openapi.yml
  format: yaml
  label: Compeller Renderings API
  slug: compeller-ai-renderings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-renderings-api-openapi.yml
- filename: compeller-ai-webhooks-api-openapi.yml
  format: yaml
  label: Compeller Webhooks API
  slug: compeller-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Compeller Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compeller secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Compeller
provider_slug: compeller-ai
scheme_count: 2
schemes:
- bearerFormat: opaque
  description: 'Compeller API token sent as `Authorization: Bearer <token>`.'
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/compeller-ai-openapi.yml
  type: http
- description: 'Compeller API token sent as `X-API-Token: <token>` (equivalent to bearer).'
  in: header
  name: apiTokenHeader
  parameter: X-API-Token
  sources:
  - openapi/compeller-ai-openapi.yml
  type: apiKey
slug: compeller-ai-authentication
source_filename: compeller-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://compeller.ai/for-agents\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: 'Compeller API token sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/compeller-ai-openapi.yml\n- name: apiTokenHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Token\n  description: 'Compeller API token sent as `X-API-Token: <token>` (equivalent to\n    bearer).'\n  sources:\n  - openapi/compeller-ai-openapi.yml\ndocs: https://compeller.ai/for-agents\nnotes:\n- 'Tokens are issued per Compeller user account and scope every request to that account\n  (for-agents page). Either Authorization: Bearer or X-API-Token is accepted on all\n  authenticated v1 and MCP calls.'\n- Docs describe token issuance via the dashboard (Account > API Access), POST /api/v1/auth/token,\n  POST /api/login (alias POST /api/v1/login)\
  \ and self-serve agent signup POST /api/v1/auth/signup.\n  These endpoints were read from docs only and never called.\n- 'Missing or invalid tokens return 401 on REST and a tool-level error (isError: true)\n  on MCP.'\n"
source_yaml_url: https://artifacts.apis.io/compeller-ai/authentication/compeller-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Music
- Video Generation
- Live Performance
- Audio Reactive Visuals
- MCP
---
