---
anonymous_access: false
api_key_in: []
api_specs:
- filename: binruleschecker-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Bin Rules Checker Enquiry API
  slug: binruleschecker-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/binruleschecker-co-uk/openapi/binruleschecker-co-uk-enquiry-api-openapi.yml
- filename: binruleschecker-co-uk-guide-api-openapi.yml
  format: yaml
  label: Bin Rules Checker Guide API
  slug: binruleschecker-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/binruleschecker-co-uk/openapi/binruleschecker-co-uk-guide-api-openapi.yml
- filename: binruleschecker-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Bin Rules Checker MCP API
  slug: binruleschecker-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/binruleschecker-co-uk/openapi/binruleschecker-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Binruleschecker Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bin Rules Checker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bin Rules Checker
provider_slug: binruleschecker-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/binruleschecker-co-uk-openapi.json
  type: http
slug: binruleschecker-co-uk-authentication
source_filename: binruleschecker-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/binruleschecker-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/binruleschecker-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/binruleschecker-co-uk/authentication/binruleschecker-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Recycling
- Waste
- United Kingdom
- Environment
- Guidance
---
