---
anonymous_access: false
api_key_in: []
api_specs:
- filename: natalchart-ai-all-plans-api-openapi.yml
  format: yaml
  label: NatalChart.AI All plans API
  slug: natalchart-ai-all-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/natalchart-ai/openapi/natalchart-ai-all-plans-api-openapi.yml
- filename: natalchart-ai-premium-and-max-api-openapi.yml
  format: yaml
  label: NatalChart.AI Premium and MAX API
  slug: natalchart-ai-premium-and-max-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/natalchart-ai/openapi/natalchart-ai-premium-and-max-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NatalChart.AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: NatalChart.AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NatalChart.AI
provider_slug: natalchart-ai
scheme_count: 1
schemes:
- description: 'Your API key: the API & MCP tab at https://www.natalchart.ai/developers/keys'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/natalchart-ai-openapi.json
  type: http
slug: natalchart-ai-authentication
source_filename: natalchart-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/natalchart-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Your API key: the API & MCP tab at https://www.natalchart.ai/developers/keys'\n  sources:\n  - openapi/natalchart-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/natalchart-ai/authentication/natalchart-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Astrology
- Artificial Intelligence
- Charts
- Free
- Swiss Ephemeris
---
