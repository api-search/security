---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commercialkitchencost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Commercial Kitchen Cost Enquiry API
  slug: commercialkitchencost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialkitchencost-co-uk/openapi/commercialkitchencost-co-uk-enquiry-api-openapi.yml
- filename: commercialkitchencost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Commercial Kitchen Cost MCP API
  slug: commercialkitchencost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialkitchencost-co-uk/openapi/commercialkitchencost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Commercial Kitchen Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commercial Kitchen Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commercial Kitchen Cost
provider_slug: commercialkitchencost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/commercialkitchencost-co-uk-openapi.yml
  type: http
slug: commercialkitchencost-co-uk-authentication
source_filename: commercialkitchencost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/commercialkitchencost-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with\n    it; the bulk entity export requires one.'\n  sources:\n  - openapi/commercialkitchencost-co-uk-openapi.yml\ndocs: https://commercialkitchencost.co.uk/mcp\nnote: 'The MCP server card (GET /mcp, 200, 2026-11-04) declares \"auth\": \"none\"; the\n  OpenAPI makes the emk_ bearer key optional (free tier without it). No auth documentation\n  page exists; docs/MCP.md referenced by the spec returns 404.'\n"
source_yaml_url: https://artifacts.apis.io/commercialkitchencost-co-uk/authentication/commercialkitchencost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Commercial Kitchens
- Fit-Out
- Hospitality
- Cost Data
- Quotes
- United Kingdom
---
