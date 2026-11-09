---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crmtrades-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: CRM for Trades Enquiry API
  slug: crmtrades-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crmtrades-co-uk/openapi/crmtrades-co-uk-enquiry-api-openapi.yml
- filename: crmtrades-co-uk-mcp-api-openapi.yml
  format: yaml
  label: CRM for Trades MCP API
  slug: crmtrades-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crmtrades-co-uk/openapi/crmtrades-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crmtrades Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CRM for Trades secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CRM for Trades
provider_slug: crmtrades-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/crmtrades-co-uk-openapi.json
  type: http
slug: crmtrades-co-uk-authentication
source_filename: crmtrades-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/crmtrades-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/crmtrades-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/crmtrades-co-uk/authentication/crmtrades-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Trade Software
- Job Management
- Quotes
- Scheduling
---
