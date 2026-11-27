---
anonymous_access: false
api_key_in: []
api_specs:
- filename: epcupgradecost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: EPC Upgrade Cost Enquiry API
  slug: epcupgradecost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epcupgradecost-co-uk/openapi/epcupgradecost-co-uk-enquiry-api-openapi.yml
- filename: epcupgradecost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: EPC Upgrade Cost MCP API
  slug: epcupgradecost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epcupgradecost-co-uk/openapi/epcupgradecost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: EPC Upgrade Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: EPC Upgrade Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EPC Upgrade Cost
provider_slug: epcupgradecost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/epcupgradecost-co-uk-openapi.json
  type: http
slug: epcupgradecost-co-uk-authentication
source_filename: epcupgradecost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/epcupgradecost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/epcupgradecost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/epcupgradecost-co-uk/authentication/epcupgradecost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Real Estate
- Landlords
- United Kingdom
---
