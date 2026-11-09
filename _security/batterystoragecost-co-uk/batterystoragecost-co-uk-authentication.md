---
anonymous_access: false
api_key_in: []
api_specs:
- filename: batterystoragecost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Battery Storage Cost Enquiry API
  slug: batterystoragecost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/batterystoragecost-co-uk/openapi/batterystoragecost-co-uk-enquiry-api-openapi.yml
- filename: batterystoragecost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Battery Storage Cost MCP API
  slug: batterystoragecost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/batterystoragecost-co-uk/openapi/batterystoragecost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Batterystoragecost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Battery Storage Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Battery Storage Cost
provider_slug: batterystoragecost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/batterystoragecost-co-uk-openapi.json
  type: http
slug: batterystoragecost-co-uk-authentication
source_filename: batterystoragecost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/batterystoragecost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/batterystoragecost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/batterystoragecost-co-uk/authentication/batterystoragecost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Battery
- Storage
- United Kingdom
- Cost
---
