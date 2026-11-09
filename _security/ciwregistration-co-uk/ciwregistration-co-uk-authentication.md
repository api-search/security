---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ciwregistration-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: CIW Registration Enquiry API
  slug: ciwregistration-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ciwregistration-co-uk/openapi/ciwregistration-co-uk-enquiry-api-openapi.yml
- filename: ciwregistration-co-uk-mcp-api-openapi.yml
  format: yaml
  label: CIW Registration MCP API
  slug: ciwregistration-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ciwregistration-co-uk/openapi/ciwregistration-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ciwregistration Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CIW Registration secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CIW Registration
provider_slug: ciwregistration-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/ciwregistration-co-uk-openapi.json
  type: http
slug: ciwregistration-co-uk-authentication
source_filename: ciwregistration-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/ciwregistration-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/ciwregistration-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ciwregistration-co-uk/authentication/ciwregistration-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Wales
- Registration
- Social Care
- Information Services
---
