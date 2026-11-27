---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adrcourses-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: ADR Courses Enquiry API
  slug: adrcourses-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrcourses-co-uk/openapi/adrcourses-co-uk-enquiry-api-openapi.yml
- filename: adrcourses-co-uk-mcp-api-openapi.yml
  format: yaml
  label: ADR Courses MCP API
  slug: adrcourses-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrcourses-co-uk/openapi/adrcourses-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ADR Courses Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADR Courses secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ADR Courses
provider_slug: adrcourses-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/adrcourses-co-uk-openapi.json
  type: http
slug: adrcourses-co-uk-authentication
source_filename: adrcourses-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/adrcourses-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/adrcourses-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/adrcourses-co-uk/authentication/adrcourses-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- ADR
- Training
- United Kingdom
- Transportation
- Safety
---
