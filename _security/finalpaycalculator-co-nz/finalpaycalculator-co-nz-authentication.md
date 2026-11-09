---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finalpaycalculator-co-nz-calculator-api-openapi.yml
  format: yaml
  label: Final Pay Calculator NZ Calculator API
  slug: finalpaycalculator-co-nz-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finalpaycalculator-co-nz/openapi/finalpaycalculator-co-nz-calculator-api-openapi.yml
- filename: finalpaycalculator-co-nz-enquiry-api-openapi.yml
  format: yaml
  label: Final Pay Calculator NZ Enquiry API
  slug: finalpaycalculator-co-nz-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finalpaycalculator-co-nz/openapi/finalpaycalculator-co-nz-enquiry-api-openapi.yml
- filename: finalpaycalculator-co-nz-mcp-api-openapi.yml
  format: yaml
  label: Final Pay Calculator NZ MCP API
  slug: finalpaycalculator-co-nz-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finalpaycalculator-co-nz/openapi/finalpaycalculator-co-nz-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Finalpaycalculator Co Nz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Final Pay Calculator NZ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Final Pay Calculator NZ
provider_slug: finalpaycalculator-co-nz
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/finalpaycalculator-co-nz-openapi.json
  type: http
slug: finalpaycalculator-co-nz-authentication
source_filename: finalpaycalculator-co-nz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/finalpaycalculator-co-nz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/finalpaycalculator-co-nz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/finalpaycalculator-co-nz/authentication/finalpaycalculator-co-nz-authentication.yml
summary_line: http · 1 scheme
tags:
- Final Pay
- Payroll
- New Zealand
- Holidays Act 2003
- Employment
- Holiday Pay
- Calculator
- MCP
---
