---
anonymous_access: false
api_key_in: []
api_specs:
- filename: currentannuityrates-co-uk-calculator-api-openapi.yml
  format: yaml
  label: Current Annuity Rates Calculator API
  slug: currentannuityrates-co-uk-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/currentannuityrates-co-uk/openapi/currentannuityrates-co-uk-calculator-api-openapi.yml
- filename: currentannuityrates-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Current Annuity Rates Enquiry API
  slug: currentannuityrates-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/currentannuityrates-co-uk/openapi/currentannuityrates-co-uk-enquiry-api-openapi.yml
- filename: currentannuityrates-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Current Annuity Rates MCP API
  slug: currentannuityrates-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/currentannuityrates-co-uk/openapi/currentannuityrates-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Current Annuity Rates Authentication
name_suffix: Authentication
oauth_flows: []
overview: Current Annuity Rates secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Current Annuity Rates
provider_slug: currentannuityrates-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/currentannuityrates-co-uk-openapi.yml
  - https://currentannuityrates.co.uk/openapi.json
  type: http
slug: currentannuityrates-co-uk-authentication
source_filename: currentannuityrates-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://currentannuityrates.co.uk/openapi.json\ndocs: https://currentannuityrates.co.uk/mcp\nsummary:\n  types:\n  - http\n  optional: true\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  required: false\n  sources:\n  - openapi/currentannuityrates-co-uk-openapi.yml\n  - https://currentannuityrates.co.uk/openapi.json\nmcp:\n  endpoint: https://currentannuityrates.co.uk/mcp\n  auth: none\n  source: https://currentannuityrates.co.uk/mcp\n  note: >-\n    The GET /mcp server card (HTTP 200, fetched 2026-11-04) declares \"auth\": \"none\". The OpenAPI defines the bearer\n    access key as optional (no top-level security requirement); it raises the 429 ceiling. No page found documents how to\n    obtain an emk_ key; the 429 description references docs/MCP.md, which is not published on\
  \ the site (/docs/ returned 404).\n"
source_yaml_url: https://artifacts.apis.io/currentannuityrates-co-uk/authentication/currentannuityrates-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Annuities
- Pensions
- Retirement Income
- Personal Finance
- United Kingdom
- Calculators
- MCP
---
