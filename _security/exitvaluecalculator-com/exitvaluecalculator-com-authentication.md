---
anonymous_access: false
api_key_in: []
api_specs:
- filename: exitvaluecalculator-com-calculator-api-openapi.yml
  format: yaml
  label: Exit Value Calculator Calculator API
  slug: exitvaluecalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvaluecalculator-com/openapi/exitvaluecalculator-com-calculator-api-openapi.yml
- filename: exitvaluecalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: Exit Value Calculator Enquiry API
  slug: exitvaluecalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvaluecalculator-com/openapi/exitvaluecalculator-com-enquiry-api-openapi.yml
- filename: exitvaluecalculator-com-mcp-api-openapi.yml
  format: yaml
  label: Exit Value Calculator MCP API
  slug: exitvaluecalculator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvaluecalculator-com/openapi/exitvaluecalculator-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Exit Value Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exit Value Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exit Value Calculator
provider_slug: exitvaluecalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/exitvaluecalculator-com-openapi.json
  type: http
slug: exitvaluecalculator-com-authentication
source_filename: exitvaluecalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/exitvaluecalculator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/exitvaluecalculator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/exitvaluecalculator-com/authentication/exitvaluecalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Tax
- Calculator
- United Kingdom
---
