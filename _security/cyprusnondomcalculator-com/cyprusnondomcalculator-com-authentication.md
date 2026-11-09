---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cyprusnondomcalculator-com-calculator-api-openapi.yml
  format: yaml
  label: Cyprus Non-Dom Calculator Calculator API
  slug: cyprusnondomcalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyprusnondomcalculator-com/openapi/cyprusnondomcalculator-com-calculator-api-openapi.yml
- filename: cyprusnondomcalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: Cyprus Non-Dom Calculator Enquiry API
  slug: cyprusnondomcalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyprusnondomcalculator-com/openapi/cyprusnondomcalculator-com-enquiry-api-openapi.yml
- filename: cyprusnondomcalculator-com-mcp-api-openapi.yml
  format: yaml
  label: Cyprus Non-Dom Calculator MCP API
  slug: cyprusnondomcalculator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyprusnondomcalculator-com/openapi/cyprusnondomcalculator-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cyprusnondomcalculator Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyprus Non-Dom Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cyprus Non-Dom Calculator
provider_slug: cyprusnondomcalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cyprusnondomcalculator-com-openapi.yml
  type: http
slug: cyprusnondomcalculator-com-authentication
source_filename: cyprusnondomcalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/cyprusnondomcalculator-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cyprusnondomcalculator-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cyprusnondomcalculator-com/authentication/cyprusnondomcalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Tax
- Cyprus
- Calculators
- Personal Finance
- Non-Dom
- MCP
---
