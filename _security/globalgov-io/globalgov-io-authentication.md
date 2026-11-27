---
anonymous_access: false
api_key_in: []
api_specs:
- filename: globalgov-io-agencies-api-openapi.yml
  format: yaml
  label: GlobalGov Agencies API
  slug: globalgov-io-agencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-agencies-api-openapi.yml
- filename: globalgov-io-awards-api-openapi.yml
  format: yaml
  label: GlobalGov Awards API
  slug: globalgov-io-awards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-awards-api-openapi.yml
- filename: globalgov-io-meta-api-openapi.yml
  format: yaml
  label: GlobalGov Meta API
  slug: globalgov-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-meta-api-openapi.yml
- filename: globalgov-io-solicitations-api-openapi.yml
  format: yaml
  label: GlobalGov Solicitations API
  slug: globalgov-io-solicitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-solicitations-api-openapi.yml
- filename: globalgov-io-vendors-api-openapi.yml
  format: yaml
  label: GlobalGov Vendors API
  slug: globalgov-io-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalgov-io/openapi/globalgov-io-vendors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GlobalGov Authentication
name_suffix: Authentication
oauth_flows: []
overview: GlobalGov secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GlobalGov
provider_slug: globalgov-io
scheme_count: 1
schemes:
- bearerFormat: ggk_live_...
  description: API key from Settings -> API & MCP Access
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/globalgov-io-openapi.json
  type: http
slug: globalgov-io-authentication
source_filename: globalgov-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/globalgov-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ggk_live_...\n  description: API key from Settings -> API & MCP Access\n  sources:\n  - openapi/globalgov-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/globalgov-io/authentication/globalgov-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Procurement
- B2B
- Intelligence
- Platform
---
