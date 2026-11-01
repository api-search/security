---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eorcompass-com-dataset-api-openapi.yml
  format: yaml
  label: eorcompass-com Dataset API
  slug: eorcompass-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eorcompass-com/openapi/eorcompass-com-dataset-api-openapi.yml
- filename: eorcompass-com-enquiry-api-openapi.yml
  format: yaml
  label: eorcompass-com Enquiry API
  slug: eorcompass-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eorcompass-com/openapi/eorcompass-com-enquiry-api-openapi.yml
- filename: eorcompass-com-mcp-api-openapi.yml
  format: yaml
  label: eorcompass-com MCP API
  slug: eorcompass-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eorcompass-com/openapi/eorcompass-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eorcompass Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: eorcompass-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: eorcompass-com
provider_slug: eorcompass-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/eorcompass-com-openapi.json
  - openapi/eorcompass-com-openapi.yml
  type: http
slug: eorcompass-com-authentication
source_filename: eorcompass-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/eorcompass-com-openapi.json, openapi/eorcompass-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/eorcompass-com-openapi.json\n  - openapi/eorcompass-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/eorcompass-com/authentication/eorcompass-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- EmployerOfRecord
- Payroll
- PricingComparison
- HRTech
---
