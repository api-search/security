---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commercialmortgagecalculator-uk-calculator-api-openapi.yml
  format: yaml
  label: Commercial Mortgage Calculator Calculator API
  slug: commercialmortgagecalculator-uk-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialmortgagecalculator-uk/openapi/commercialmortgagecalculator-uk-calculator-api-openapi.yml
- filename: commercialmortgagecalculator-uk-enquiry-api-openapi.yml
  format: yaml
  label: Commercial Mortgage Calculator Enquiry API
  slug: commercialmortgagecalculator-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialmortgagecalculator-uk/openapi/commercialmortgagecalculator-uk-enquiry-api-openapi.yml
- filename: commercialmortgagecalculator-uk-mcp-api-openapi.yml
  format: yaml
  label: Commercial Mortgage Calculator MCP API
  slug: commercialmortgagecalculator-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialmortgagecalculator-uk/openapi/commercialmortgagecalculator-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commercial Mortgage Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commercial Mortgage Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commercial Mortgage Calculator
provider_slug: commercialmortgagecalculator-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/commercialmortgagecalculator-uk-openapi.yml
  type: http
slug: commercialmortgagecalculator-uk-authentication
source_filename: commercialmortgagecalculator-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commercialmortgagecalculator.uk/openapi.json\ndocs: https://commercialmortgagecalculator.uk/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  required: false\n  key_prefix: emk_\n  sources:\n  - openapi/commercialmortgagecalculator-uk-openapi.yml\nnote: 'The MCP card (GET https://commercialmortgagecalculator.uk/mcp, HTTP 200) declares \"auth\": \"none\" for the Streamable HTTP MCP endpoint; the OpenAPI makes the\n  bearer access key optional (free tier without it). No page documents how to obtain an emk_ key; the 429 description\n  references docs/MCP.md, which returned 404 at https://commercialmortgagecalculator.uk/docs/MCP.md.'\n"
source_yaml_url: https://artifacts.apis.io/commercialmortgagecalculator-uk/authentication/commercialmortgagecalculator-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Commercial Mortgages
- Mortgage Calculator
- Commercial Property
- United Kingdom
- Finance
- Lending
- MCP
---
