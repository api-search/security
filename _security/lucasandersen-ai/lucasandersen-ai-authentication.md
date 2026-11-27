---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lucasandersen-ai-basis-api-openapi.yml
  format: yaml
  label: Lucas Andersen Basis API
  slug: lucasandersen-ai-basis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucasandersen-ai/openapi/lucasandersen-ai-basis-api-openapi.yml
- filename: lucasandersen-ai-mcp-api-openapi.yml
  format: yaml
  label: Lucas Andersen MCP API
  slug: lucasandersen-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucasandersen-ai/openapi/lucasandersen-ai-mcp-api-openapi.yml
- filename: lucasandersen-ai-mlp-api-openapi.yml
  format: yaml
  label: Lucas Andersen Mlp API
  slug: lucasandersen-ai-mlp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucasandersen-ai/openapi/lucasandersen-ai-mlp-api-openapi.yml
- filename: lucasandersen-ai-reference-api-openapi.yml
  format: yaml
  label: Lucas Andersen Reference API
  slug: lucasandersen-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucasandersen-ai/openapi/lucasandersen-ai-reference-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lucas Andersen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucas Andersen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lucas Andersen
provider_slug: lucasandersen-ai
scheme_count: 1
schemes:
- description: API key as Bearer token. Unauthenticated requests permitted at lower rate limit (10/day per IP).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lucasandersen-ai-openapi.json
  type: http
slug: lucasandersen-ai-authentication
source_filename: lucasandersen-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lucasandersen-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key as Bearer token. Unauthenticated requests permitted at lower rate limit\n    (10/day per IP).\n  sources:\n  - openapi/lucasandersen-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lucasandersen-ai/authentication/lucasandersen-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Tax
- MLP
- Tools
---
