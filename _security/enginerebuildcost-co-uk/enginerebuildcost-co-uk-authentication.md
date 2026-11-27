---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enginerebuildcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Engine Rebuild Cost Enquiry API
  slug: enginerebuildcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enginerebuildcost-co-uk/openapi/enginerebuildcost-co-uk-enquiry-api-openapi.yml
- filename: enginerebuildcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Engine Rebuild Cost MCP API
  slug: enginerebuildcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enginerebuildcost-co-uk/openapi/enginerebuildcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Engine Rebuild Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Engine Rebuild Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Engine Rebuild Cost
provider_slug: enginerebuildcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/enginerebuildcost-co-uk-openapi.yml
  type: http
slug: enginerebuildcost-co-uk-authentication
source_filename: enginerebuildcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/enginerebuildcost-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/enginerebuildcost-co-uk-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/enginerebuildcost-co-uk/authentication/enginerebuildcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automotive
- Engine
- Rebuild
- United Kingdom
- Cost
---
