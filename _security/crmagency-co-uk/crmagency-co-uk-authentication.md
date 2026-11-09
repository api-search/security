---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crmagency-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: CRM Agency Enquiry API
  slug: crmagency-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crmagency-co-uk/openapi/crmagency-co-uk-enquiry-api-openapi.yml
- filename: crmagency-co-uk-mcp-api-openapi.yml
  format: yaml
  label: CRM Agency MCP API
  slug: crmagency-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crmagency-co-uk/openapi/crmagency-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crmagency Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CRM Agency secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CRM Agency
provider_slug: crmagency-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/crmagency-co-uk-openapi.json
  type: http
slug: crmagency-co-uk-authentication
source_filename: crmagency-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/crmagency-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/crmagency-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/crmagency-co-uk/authentication/crmagency-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Agency
- United Kingdom
- Software-as-a-Service
- Consulting
---
