---
anonymous_access: true
api_key_in: []
api_specs:
- filename: corptaxcalculator-co-uk-dataset-api-openapi.yml
  format: yaml
  label: Corp Tax Calculator Dataset API
  slug: corptaxcalculator-co-uk-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corptaxcalculator-co-uk/openapi/corptaxcalculator-co-uk-dataset-api-openapi.yml
- filename: corptaxcalculator-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Corp Tax Calculator Enquiry API
  slug: corptaxcalculator-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corptaxcalculator-co-uk/openapi/corptaxcalculator-co-uk-enquiry-api-openapi.yml
- filename: corptaxcalculator-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Corp Tax Calculator MCP API
  slug: corptaxcalculator-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corptaxcalculator-co-uk/openapi/corptaxcalculator-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Corp Tax Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corp Tax Calculator secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Corp Tax Calculator
provider_slug: corptaxcalculator-co-uk
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/corptaxcalculator-co-uk-openapi.yml
  type: http
- description: MCP endpoint advertises "auth":"none" (stateless, JSON responses) in its server card.
  name: none
  sources:
  - https://corptaxcalculator.co.uk/mcp
  type: none
slug: corptaxcalculator-co-uk-authentication
source_filename: corptaxcalculator-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corptaxcalculator.co.uk/mcp\ndocs: https://corptaxcalculator.co.uk/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\n  note: The MCP server card (GET https://corptaxcalculator.co.uk/mcp, HTTP 200, generated 2026-11-03) declares \"auth\":\"none\"\n    for the Streamable HTTP endpoint; the OpenAPI declares an optional bearer access key (emk_...). No key-issuance, OAuth\n    or scopes documentation was found (/docs/MCP.md, referenced by the spec's 429 description, returns 404).\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  key_prefix: emk_\n  required: false\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'\n  sources:\n  - openapi/corptaxcalculator-co-uk-openapi.yml\n- name: none\n  type: none\n  description: MCP endpoint advertises \"auth\":\"none\" (stateless, JSON responses) in its server card.\n  sources:\n  -\
  \ https://corptaxcalculator.co.uk/mcp\n"
source_yaml_url: https://artifacts.apis.io/corptaxcalculator-co-uk/authentication/corptaxcalculator-co-uk-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Corporation Tax
- Tax Calculator
- United Kingdom
- R&D Tax Relief
- Capital Allowances
- Datasets
---
