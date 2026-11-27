---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cyprusgrosstonet-com-calculator-api-openapi.yml
  format: yaml
  label: Cyprus Gross to Net Calculator API
  slug: cyprusgrosstonet-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyprusgrosstonet-com/openapi/cyprusgrosstonet-com-calculator-api-openapi.yml
- filename: cyprusgrosstonet-com-enquiry-api-openapi.yml
  format: yaml
  label: Cyprus Gross to Net Enquiry API
  slug: cyprusgrosstonet-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyprusgrosstonet-com/openapi/cyprusgrosstonet-com-enquiry-api-openapi.yml
- filename: cyprusgrosstonet-com-mcp-api-openapi.yml
  format: yaml
  label: Cyprus Gross to Net MCP API
  slug: cyprusgrosstonet-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyprusgrosstonet-com/openapi/cyprusgrosstonet-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cyprus Gross to Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyprus Gross to Net secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cyprus Gross to Net
provider_slug: cyprusgrosstonet-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cyprusgrosstonet-com-openapi.yml
  type: http
slug: cyprusgrosstonet-com-authentication
source_filename: cyprusgrosstonet-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cyprusgrosstonet-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cyprusgrosstonet-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cyprusgrosstonet-com/authentication/cyprusgrosstonet-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Payroll
- Tax Calculator
- Cyprus
---
