---
api_key_in: []
api_specs:
- filename: motorola-solutions-motorola-api-openapi.yml
  format: yaml
  label: Motorola Solutions API
  slug: motorola-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motorola-solutions/refs/heads/main/openapi/motorola-solutions-motorola-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Motorola Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Motorola Solutions secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Motorola Solutions
provider_slug: motorola-solutions
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/motorola-solutions-motorola-api-openapi.yml
  type: http
slug: motorola-solutions-authentication
source_filename: motorola-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/motorola-solutions-motorola-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/motorola-solutions-motorola-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motorola-solutions/refs/heads/main/authentication/motorola-solutions-authentication.yml
summary_line: http · 1 scheme
tags:
- Public Safety
- Communications
- Video Security
- IoT
- Fortune 500
---
