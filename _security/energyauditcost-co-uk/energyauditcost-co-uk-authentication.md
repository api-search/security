---
anonymous_access: false
api_key_in: []
api_specs:
- filename: energyauditcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Energy Audit Cost Enquiry API
  slug: energyauditcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/energyauditcost-co-uk/openapi/energyauditcost-co-uk-enquiry-api-openapi.yml
- filename: energyauditcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Energy Audit Cost MCP API
  slug: energyauditcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/energyauditcost-co-uk/openapi/energyauditcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Energy Audit Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Energy Audit Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Energy Audit Cost
provider_slug: energyauditcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/energyauditcost-co-uk-openapi.json
  type: http
slug: energyauditcost-co-uk-authentication
source_filename: energyauditcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/energyauditcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/energyauditcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/energyauditcost-co-uk/authentication/energyauditcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Audit
- United Kingdom
- Pricing
- Data
---
