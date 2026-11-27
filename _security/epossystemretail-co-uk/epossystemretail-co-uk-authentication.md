---
anonymous_access: false
api_key_in: []
api_specs:
- filename: epossystemretail-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: EPOS System for Retail Enquiry API
  slug: epossystemretail-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epossystemretail-co-uk/openapi/epossystemretail-co-uk-enquiry-api-openapi.yml
- filename: epossystemretail-co-uk-mcp-api-openapi.yml
  format: yaml
  label: EPOS System for Retail MCP API
  slug: epossystemretail-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epossystemretail-co-uk/openapi/epossystemretail-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: EPOS System for Retail Authentication
name_suffix: Authentication
oauth_flows: []
overview: EPOS System for Retail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EPOS System for Retail
provider_slug: epossystemretail-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/epossystemretail-co-uk-openapi.json
  type: http
slug: epossystemretail-co-uk-authentication
source_filename: epossystemretail-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/epossystemretail-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/epossystemretail-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/epossystemretail-co-uk/authentication/epossystemretail-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- EPOS
- Retail
- Point-of-Sale
- United Kingdom
---
