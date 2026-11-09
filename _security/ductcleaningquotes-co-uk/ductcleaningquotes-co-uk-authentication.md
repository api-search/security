---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ductcleaningquotes-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Duct Cleaning Quotes Enquiry API
  slug: ductcleaningquotes-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ductcleaningquotes-co-uk/openapi/ductcleaningquotes-co-uk-enquiry-api-openapi.yml
- filename: ductcleaningquotes-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Duct Cleaning Quotes MCP API
  slug: ductcleaningquotes-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ductcleaningquotes-co-uk/openapi/ductcleaningquotes-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ductcleaningquotes Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duct Cleaning Quotes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duct Cleaning Quotes
provider_slug: ductcleaningquotes-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/ductcleaningquotes-co-uk-openapi.json
  type: http
slug: ductcleaningquotes-co-uk-authentication
source_filename: ductcleaningquotes-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/ductcleaningquotes-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/ductcleaningquotes-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ductcleaningquotes-co-uk/authentication/ductcleaningquotes-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Duct Cleaning
- United Kingdom
- Home Services
- Quotes
- Commercial
---
