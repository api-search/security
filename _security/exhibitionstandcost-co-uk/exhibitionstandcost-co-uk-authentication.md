---
anonymous_access: false
api_key_in: []
api_specs:
- filename: exhibitionstandcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Exhibition Stand Cost Enquiry API
  slug: exhibitionstandcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exhibitionstandcost-co-uk/openapi/exhibitionstandcost-co-uk-enquiry-api-openapi.yml
- filename: exhibitionstandcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Exhibition Stand Cost MCP API
  slug: exhibitionstandcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exhibitionstandcost-co-uk/openapi/exhibitionstandcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Exhibition Stand Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exhibition Stand Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exhibition Stand Cost
provider_slug: exhibitionstandcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/exhibitionstandcost-co-uk-openapi.json
  type: http
slug: exhibitionstandcost-co-uk-authentication
source_filename: exhibitionstandcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/exhibitionstandcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/exhibitionstandcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/exhibitionstandcost-co-uk/authentication/exhibitionstandcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Exhibition
- Stand
- Cost
- United Kingdom
- Builder
---
