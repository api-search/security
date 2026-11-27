---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lexbase-pt-diploma-api-openapi.yml
  format: yaml
  label: Lexbase Diploma API
  slug: lexbase-pt-diploma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-diploma-api-openapi.yml
- filename: lexbase-pt-diplomas-api-openapi.yml
  format: yaml
  label: Lexbase Diplomas API
  slug: lexbase-pt-diplomas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-diplomas-api-openapi.yml
- filename: lexbase-pt-fragment-api-openapi.yml
  format: yaml
  label: Lexbase Fragment API
  slug: lexbase-pt-fragment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-fragment-api-openapi.yml
- filename: lexbase-pt-health-api-openapi.yml
  format: yaml
  label: Lexbase Health API
  slug: lexbase-pt-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-health-api-openapi.yml
- filename: lexbase-pt-search-api-openapi.yml
  format: yaml
  label: Lexbase Search API
  slug: lexbase-pt-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-search-api-openapi.yml
- filename: lexbase-pt-themes-api-openapi.yml
  format: yaml
  label: Lexbase Themes API
  slug: lexbase-pt-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-themes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lexbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lexbase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lexbase
provider_slug: lexbase-pt
scheme_count: 1
schemes:
- description: A Lexbase API key (lx_… / leis_…) in the Authorization header. Create one at https://lexbase.pt/mcp.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lexbase-pt-openapi.json
  type: http
slug: lexbase-pt-authentication
source_filename: lexbase-pt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lexbase-pt-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A Lexbase API key (lx_… / leis_…) in the Authorization header. Create one at\n    https://lexbase.pt/mcp.\n  sources:\n  - openapi/lexbase-pt-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lexbase-pt/authentication/lexbase-pt-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal Tech
- PortugueseLaw
- Search
- AI Integration
---
