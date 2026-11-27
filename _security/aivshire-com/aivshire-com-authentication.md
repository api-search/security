---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aivshire-com-calculator-api-openapi.yml
  format: yaml
  label: AI vs Hire Calculator API
  slug: aivshire-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivshire-com/openapi/aivshire-com-calculator-api-openapi.yml
- filename: aivshire-com-enquiry-api-openapi.yml
  format: yaml
  label: AI vs Hire Enquiry API
  slug: aivshire-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivshire-com/openapi/aivshire-com-enquiry-api-openapi.yml
- filename: aivshire-com-mcp-api-openapi.yml
  format: yaml
  label: AI vs Hire MCP API
  slug: aivshire-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivshire-com/openapi/aivshire-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AI vs Hire Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI vs Hire secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AI vs Hire
provider_slug: aivshire-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/aivshire-com-openapi.json
  type: http
slug: aivshire-com-authentication
source_filename: aivshire-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aivshire-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/aivshire-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aivshire-com/authentication/aivshire-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Hiring
- Cost Comparison
- Finance
- Automation
---
