---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bolotstudio-com-authentication-api-openapi.yml
  format: yaml
  label: Bolot Studio Authentication API
  slug: bolotstudio-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolotstudio-com/openapi/bolotstudio-com-authentication-api-openapi.yml
- filename: bolotstudio-com-discovery-api-openapi.yml
  format: yaml
  label: Bolot Studio Discovery API
  slug: bolotstudio-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolotstudio-com/openapi/bolotstudio-com-discovery-api-openapi.yml
- filename: bolotstudio-com-feeds-api-openapi.yml
  format: yaml
  label: Bolot Studio Feeds API
  slug: bolotstudio-com-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolotstudio-com/openapi/bolotstudio-com-feeds-api-openapi.yml
- filename: bolotstudio-com-mcp-api-openapi.yml
  format: yaml
  label: Bolot Studio MCP API
  slug: bolotstudio-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolotstudio-com/openapi/bolotstudio-com-mcp-api-openapi.yml
- filename: bolotstudio-com-products-api-openapi.yml
  format: yaml
  label: Bolot Studio Products API
  slug: bolotstudio-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolotstudio-com/openapi/bolotstudio-com-products-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bolot Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bolot Studio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bolot Studio
provider_slug: bolotstudio-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Access token obtained from POST /api/ucp/auth
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bolotstudio-com-openapi.json
  type: http
slug: bolotstudio-com-authentication
source_filename: bolotstudio-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bolotstudio-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token obtained from POST /api/ucp/auth\n  sources:\n  - openapi/bolotstudio-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bolotstudio-com/authentication/bolotstudio-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Print Shop
- CustomPrints
- E-Commerce
- Photography
- Aluminium
---
