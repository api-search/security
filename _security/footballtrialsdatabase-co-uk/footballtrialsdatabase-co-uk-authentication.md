---
anonymous_access: false
api_key_in: []
api_specs:
- filename: footballtrialsdatabase-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Football Trials Database Enquiry API
  slug: footballtrialsdatabase-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/openapi/footballtrialsdatabase-co-uk-enquiry-api-openapi.yml
- filename: footballtrialsdatabase-co-uk-guide-api-openapi.yml
  format: yaml
  label: Football Trials Database Guide API
  slug: footballtrialsdatabase-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/openapi/footballtrialsdatabase-co-uk-guide-api-openapi.yml
- filename: footballtrialsdatabase-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Football Trials Database MCP API
  slug: footballtrialsdatabase-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/openapi/footballtrialsdatabase-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Footballtrialsdatabase Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Football Trials Database secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Football Trials Database
provider_slug: footballtrialsdatabase-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/footballtrialsdatabase-co-uk-openapi.json
  type: http
slug: footballtrialsdatabase-co-uk-authentication
source_filename: footballtrialsdatabase-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/footballtrialsdatabase-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/footballtrialsdatabase-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/authentication/footballtrialsdatabase-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- football trials
- academy recruitment
- non‑league clubs
- county FA
- paid trial events
---
