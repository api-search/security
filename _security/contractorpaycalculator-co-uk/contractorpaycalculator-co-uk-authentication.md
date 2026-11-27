---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contractorpaycalculator-co-uk-calculator-api-openapi.yml
  format: yaml
  label: Contractor Pay Calculator Calculator API
  slug: contractorpaycalculator-co-uk-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorpaycalculator-co-uk/openapi/contractorpaycalculator-co-uk-calculator-api-openapi.yml
- filename: contractorpaycalculator-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Contractor Pay Calculator Enquiry API
  slug: contractorpaycalculator-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorpaycalculator-co-uk/openapi/contractorpaycalculator-co-uk-enquiry-api-openapi.yml
- filename: contractorpaycalculator-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Contractor Pay Calculator MCP API
  slug: contractorpaycalculator-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorpaycalculator-co-uk/openapi/contractorpaycalculator-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Contractor Pay Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contractor Pay Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contractor Pay Calculator
provider_slug: contractorpaycalculator-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/contractorpaycalculator-co-uk-openapi.yml
  type: http
slug: contractorpaycalculator-co-uk-authentication
source_filename: contractorpaycalculator-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- openapi/contractorpaycalculator-co-uk-openapi.yml\n- https://contractorpaycalculator.co.uk/openapi.json\n- https://contractorpaycalculator.co.uk/mcp\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires\n    one.'\n  sources:\n  - openapi/contractorpaycalculator-co-uk-openapi.yml\ndocs: https://contractorpaycalculator.co.uk/mcp\noptional: true\nnote: Authentication is optional. The OpenAPI declares one http bearer scheme (accessKey, \"emk_...\" keys) but sets\n  no global or per-operation security requirement; the description says \"free tier without it, a named budget with\n  it\". The MCP card at /mcp states \"auth\":\"none\" for the MCP endpoint. No page documents how to obtain an access\n  key; docs/MCP.md, referenced by the 429 response description, returned HTTP\
  \ 404 at https://contractorpaycalculator.co.uk/docs/MCP.md\n  (2026-11-04).\n"
source_yaml_url: https://artifacts.apis.io/contractorpaycalculator-co-uk/authentication/contractorpaycalculator-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Calculators
- IR35
- Contractors
- Payroll
- Tax
- United Kingdom
- Umbrella Companies
---
