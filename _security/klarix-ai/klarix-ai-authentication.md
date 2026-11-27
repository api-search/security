---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: klarix-ai-competitive-intelligence-api-openapi.yml
  format: yaml
  label: Klarix Competitive intelligence API
  slug: klarix-ai-competitive-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klarix-ai/openapi/klarix-ai-competitive-intelligence-api-openapi.yml
- filename: klarix-ai-diagnostics-api-openapi.yml
  format: yaml
  label: Klarix Diagnostics API
  slug: klarix-ai-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klarix-ai/openapi/klarix-ai-diagnostics-api-openapi.yml
- filename: klarix-ai-prospect-universe-api-openapi.yml
  format: yaml
  label: Klarix Prospect universe API
  slug: klarix-ai-prospect-universe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klarix-ai/openapi/klarix-ai-prospect-universe-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Klarix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klarix secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Klarix
provider_slug: klarix-ai
scheme_count: 2
schemes:
- description: 'Klarix key, e.g. `Authorization: Bearer klx_live_…`. Get one at https://klarix.ai/mcp#get-key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/klarix-ai-openapi.json
  type: http
- description: Same key, for callers behind a proxy that strips `Authorization`. Keys on the query string are rejected.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/klarix-ai-openapi.json
  type: apiKey
slug: klarix-ai-authentication
source_filename: klarix-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/klarix-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Klarix key, e.g. `Authorization: Bearer klx_live_…`. Get one at https://klarix.ai/mcp#get-key.'\n  sources:\n  - openapi/klarix-ai-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Same key, for callers behind a proxy that strips `Authorization`. Keys on the\n    query string are rejected.\n  sources:\n  - openapi/klarix-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/klarix-ai/authentication/klarix-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Competitive Intelligence
- Software-as-a-Service
- Manufacturing
- Recruiting
- Fintech
- Healthcare
- Logistics
- Energy
---
