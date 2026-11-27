---
anonymous_access: false
api_key_in: []
api_specs:
- filename: suedeai-ai-a2a-api-openapi.yml
  format: yaml
  label: Suede A2a API
  slug: suedeai-ai-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-a2a-api-openapi.yml
- filename: suedeai-ai-agents-api-openapi.yml
  format: yaml
  label: Suede Agents API
  slug: suedeai-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-agents-api-openapi.yml
- filename: suedeai-ai-ap2-api-openapi.yml
  format: yaml
  label: Suede Ap2 API
  slug: suedeai-ai-ap2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-ap2-api-openapi.yml
- filename: suedeai-ai-catalog-api-openapi.yml
  format: yaml
  label: Suede Catalog API
  slug: suedeai-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-catalog-api-openapi.yml
- filename: suedeai-ai-mcp-api-openapi.yml
  format: yaml
  label: Suede MCP API
  slug: suedeai-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-mcp-api-openapi.yml
- filename: suedeai-ai-services-api-openapi.yml
  format: yaml
  label: Suede Services API
  slug: suedeai-ai-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-services-api-openapi.yml
- filename: suedeai-ai-suedelabs-api-openapi.yml
  format: yaml
  label: Suede Suede Labs API
  slug: suedeai-ai-suedelabs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-suedelabs-api-openapi.yml
- filename: suedeai-ai-well-known-api-openapi.yml
  format: yaml
  label: Suede .well Known API
  slug: suedeai-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suedeai-ai/openapi/suedeai-ai-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Suede Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suede secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Suede
provider_slug: suedeai-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Skyfire pay+jwt or kya-pay+jwt token issued by Skyfire and verified against https://app.skyfire.xyz/.well-known/jwks.json. Pass in the PAYMENT-SIGNATURE header.
  name: SkyfireJWT
  scheme: bearer
  sources:
  - openapi/api-openapi.json
  - openapi/suedeai-ai-openapi.json
  type: http
slug: suedeai-ai-authentication
source_filename: suedeai-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/api-openapi.json, openapi/suedeai-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: SkyfireJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Skyfire pay+jwt or kya-pay+jwt token issued by Skyfire and verified against https://app.skyfire.xyz/.well-known/jwks.json.\n    Pass in the PAYMENT-SIGNATURE header.\n  sources:\n  - openapi/api-openapi.json\n  - openapi/suedeai-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/suedeai-ai/authentication/suedeai-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Engineering
- Digital Marketing
- White‑Label Platforms
- Search Optimization
- Business Automation
- Agency Services
---
