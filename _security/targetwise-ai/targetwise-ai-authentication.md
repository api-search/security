---
anonymous_access: false
api_key_in: []
api_specs:
- filename: targetwise-ai-account-api-openapi.yml
  format: yaml
  label: targetwise-ai Account API
  slug: targetwise-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-account-api-openapi.yml
- filename: targetwise-ai-autocomplete-api-openapi.yml
  format: yaml
  label: targetwise-ai Autocomplete API
  slug: targetwise-ai-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-autocomplete-api-openapi.yml
- filename: targetwise-ai-companies-api-openapi.yml
  format: yaml
  label: targetwise-ai Companies API
  slug: targetwise-ai-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-companies-api-openapi.yml
- filename: targetwise-ai-employees-api-openapi.yml
  format: yaml
  label: targetwise-ai Employees API
  slug: targetwise-ai-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-employees-api-openapi.yml
- filename: targetwise-ai-enrichment-api-openapi.yml
  format: yaml
  label: targetwise-ai Enrichment API
  slug: targetwise-ai-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-enrichment-api-openapi.yml
- filename: targetwise-ai-prospecting-api-openapi.yml
  format: yaml
  label: targetwise-ai Prospecting API
  slug: targetwise-ai-prospecting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-prospecting-api-openapi.yml
- filename: targetwise-ai-resolution-api-openapi.yml
  format: yaml
  label: targetwise-ai Resolution API
  slug: targetwise-ai-resolution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-resolution-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Targetwise Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: targetwise-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: targetwise-ai
provider_slug: targetwise-ai
scheme_count: 1
schemes:
- bearerFormat: TargetWise API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/targetwise-ai-openapi.json
  type: http
slug: targetwise-ai-authentication
source_filename: targetwise-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/targetwise-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: TargetWise API key\n  sources:\n  - openapi/targetwise-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/targetwise-ai/authentication/targetwise-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B
- Data Enrichment
- Contact API
- MCP
- SaaS
---
