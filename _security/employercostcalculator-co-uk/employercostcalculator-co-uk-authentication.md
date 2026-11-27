---
anonymous_access: false
api_key_in: []
api_specs:
- filename: employercostcalculator-co-uk-calculator-api-openapi.yml
  format: yaml
  label: Employer Cost Calculator Calculator API
  slug: employercostcalculator-co-uk-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/employercostcalculator-co-uk/openapi/employercostcalculator-co-uk-calculator-api-openapi.yml
- filename: employercostcalculator-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Employer Cost Calculator Enquiry API
  slug: employercostcalculator-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/employercostcalculator-co-uk/openapi/employercostcalculator-co-uk-enquiry-api-openapi.yml
- filename: employercostcalculator-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Employer Cost Calculator MCP API
  slug: employercostcalculator-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/employercostcalculator-co-uk/openapi/employercostcalculator-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Employer Cost Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Employer Cost Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Employer Cost Calculator
provider_slug: employercostcalculator-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/employercostcalculator-co-uk-openapi.json
  type: http
slug: employercostcalculator-co-uk-authentication
source_filename: employercostcalculator-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/employercostcalculator-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/employercostcalculator-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/employercostcalculator-co-uk/authentication/employercostcalculator-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Calculator
- United Kingdom
- Employer
- Payroll
- Cost
---
