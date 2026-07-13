---
api_key_in:
- header
api_specs:
- filename: knack-openapi.yml
  format: yaml
  label: Knack REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knack/refs/heads/main/openapi/knack-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Knack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knack secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Knack
provider_slug: knack
scheme_count: 2
schemes:
- description: Knack Application ID identifying the target application
  in: header
  name: ApplicationId
  parameter: X-Knack-Application-Id
  sources:
  - openapi/knack-openapi.yml
  type: apiKey
- description: REST API key authorizing the request
  in: header
  name: RestApiKey
  parameter: X-Knack-REST-API-Key
  sources:
  - openapi/knack-openapi.yml
  type: apiKey
slug: knack-authentication
source_filename: knack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApplicationId\n  type: apiKey\n  in: header\n  parameter: X-Knack-Application-Id\n  description: Knack Application ID identifying the target application\n  sources:\n  - openapi/knack-openapi.yml\n- name: RestApiKey\n  type: apiKey\n  in: header\n  parameter: X-Knack-REST-API-Key\n  description: REST API key authorizing the request\n  sources:\n  - openapi/knack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knack/refs/heads/main/authentication/knack-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- No-Code
- Database
- Application Builder
- Low-Code
- Web Applications
---
