---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aifra-ru-analytics-api-openapi.yml
  format: yaml
  label: AIfra Analytics API
  slug: aifra-ru-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-analytics-api-openapi.yml
- filename: aifra-ru-health-api-openapi.yml
  format: yaml
  label: AIfra Health API
  slug: aifra-ru-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-health-api-openapi.yml
- filename: aifra-ru-mcp-api-openapi.yml
  format: yaml
  label: AIfra MCP API
  slug: aifra-ru-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-mcp-api-openapi.yml
- filename: aifra-ru-previews-api-openapi.yml
  format: yaml
  label: AIfra Previews API
  slug: aifra-ru-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-previews-api-openapi.yml
- filename: aifra-ru-ready-api-openapi.yml
  format: yaml
  label: AIfra Ready API
  slug: aifra-ru-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-ready-api-openapi.yml
- filename: aifra-ru-remote-api-openapi.yml
  format: yaml
  label: AIfra Remote API
  slug: aifra-ru-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-remote-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Aifra Ru Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIfra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIfra
provider_slug: aifra-ru
scheme_count: 1
schemes:
- bearerFormat: pmt_*
  name: managementToken
  scheme: bearer
  sources:
  - openapi/aifra-ru-openapi.json
  type: http
slug: aifra-ru-authentication
source_filename: aifra-ru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aifra-ru-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: managementToken\n  type: http\n  scheme: bearer\n  bearerFormat: pmt_*\n  sources:\n  - openapi/aifra-ru-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aifra-ru/authentication/aifra-ru-authentication.yml
summary_line: http · 1 scheme
tags:
- Software-as-a-Service
- Static-Previews
- Artificial Intelligence
- CLI
- REST
---
