---
api_key_in: []
api_specs:
- filename: index.html
  format: yaml
  label: Small Improvements REST API
  slug: small-improvements-rest-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/si-rest-api-docs/dist/index.html
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Small Improvements Authentication
name_suffix: Authentication
oauth_flows: []
overview: Small Improvements secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Small Improvements
provider_slug: small-improvements
scheme_count: 1
schemes:
- description: Personal access token generated from user profile settings
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/small-improvements-small-improvements-rest-api-openapi.yml
  type: http
slug: small-improvements-authentication
source_filename: small-improvements-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/small-improvements-small-improvements-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token generated from user profile settings\n  sources:\n  - openapi/small-improvements-small-improvements-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/small-improvements/refs/heads/main/authentication/small-improvements-authentication.yml
summary_line: http · 1 scheme
tags:
- Performance Management
- HR
- Employee Feedback
- OKRs
- 1:1 Meetings
- Pulse Surveys
- 360 Feedback
- People Management
---
