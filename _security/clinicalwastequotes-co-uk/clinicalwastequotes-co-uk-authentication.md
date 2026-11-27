---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clinicalwastequotes-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Clinical Waste Quotes Enquiry API
  slug: clinicalwastequotes-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clinicalwastequotes-co-uk/openapi/clinicalwastequotes-co-uk-enquiry-api-openapi.yml
- filename: clinicalwastequotes-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Clinical Waste Quotes MCP API
  slug: clinicalwastequotes-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clinicalwastequotes-co-uk/openapi/clinicalwastequotes-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clinical Waste Quotes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clinical Waste Quotes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clinical Waste Quotes
provider_slug: clinicalwastequotes-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/clinicalwastequotes-co-uk-openapi.yml
  type: http
slug: clinicalwastequotes-co-uk-authentication
source_filename: clinicalwastequotes-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clinicalwastequotes.co.uk/mcp\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires\n    one.'\n  sources:\n  - openapi/clinicalwastequotes-co-uk-openapi.yml\ndocs: https://clinicalwastequotes.co.uk/mcp\noptional: true\nnotes:\n- 'The OpenAPI declares the bearer access key as optional: \"free tier without it, a named budget with it\" (https://clinicalwastequotes.co.uk/openapi.json).'\n- 'The MCP server card at GET https://clinicalwastequotes.co.uk/mcp (HTTP 200, probed 2026-11-04) states \"auth\":\n  \"none\" for the MCP endpoint.'\n- No page documents how an emk_ access key is issued; the 429 description points to docs/MCP.md, which returned\n  HTTP 404 at https://clinicalwastequotes.co.uk/docs/MCP.md.\n"
source_yaml_url: https://artifacts.apis.io/clinicalwastequotes-co-uk/authentication/clinicalwastequotes-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Clinical Waste
- Waste Management
- Healthcare
- Quotes
- Lead Generation
- Compliance
- United Kingdom
---
