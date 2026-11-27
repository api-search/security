---
anonymous_access: false
api_key_in: []
api_specs:
- filename: g62-ai-searches-api-openapi.yml
  format: yaml
  label: G62 Searches API
  slug: g62-ai-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/g62-ai/openapi/g62-ai-searches-api-openapi.yml
- filename: g62-ai-status-api-openapi.yml
  format: yaml
  label: G62 Status API
  slug: g62-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/g62-ai/openapi/g62-ai-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: G62 Authentication
name_suffix: Authentication
oauth_flows: []
overview: G62 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: G62
provider_slug: g62-ai
scheme_count: 1
schemes:
- bearerFormat: G62 developer token
  description: 'Create a token from the Connect section of your G62 dashboard. Use Authorization: Bearer TOKEN. Do not place credentials in URLs.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/g62-ai-openapi.json
  type: http
slug: g62-ai-authentication
source_filename: g62-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/g62-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: G62 developer token\n  description: 'Create a token from the Connect section of your G62 dashboard. Use Authorization:\n    Bearer TOKEN. Do not place credentials in URLs.'\n  sources:\n  - openapi/g62-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/g62-ai/authentication/g62-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Patent Search
- Developer Tools
- REST
- MCP
---
