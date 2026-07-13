---
api_key_in:
- header
api_specs:
- filename: dreamfactory-system-api-openapi.yml
  format: yaml
  label: DreamFactory System API
  slug: system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-system-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dreamfactory Authentication
name_suffix: Authentication
oauth_flows: []
overview: DreamFactory secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DreamFactory
provider_slug: dreamfactory
scheme_count: 2
schemes:
- description: Session token obtained after admin login.
  in: header
  name: sessionToken
  parameter: X-DreamFactory-Session-Token
  sources:
  - openapi/dreamfactory-system-api-openapi.yml
  type: apiKey
- description: API key associated with a registered application.
  in: header
  name: apiKey
  parameter: X-DreamFactory-API-Key
  sources:
  - openapi/dreamfactory-system-api-openapi.yml
  type: apiKey
slug: dreamfactory-authentication
source_filename: dreamfactory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dreamfactory-system-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: X-DreamFactory-Session-Token\n  description: Session token obtained after admin login.\n  sources:\n  - openapi/dreamfactory-system-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-DreamFactory-API-Key\n  description: API key associated with a registered application.\n  sources:\n  - openapi/dreamfactory-system-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/authentication/dreamfactory-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
---
