---
api_key_in:
- header
api_specs:
- filename: ahasend-openapi.yml
  format: yaml
  label: AhaSend
  slug: ahasend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ahasend Authentication
name_suffix: Authentication
oauth_flows: []
overview: AhaSend secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AhaSend
provider_slug: ahasend
scheme_count: 2
schemes:
- bearerFormat: aha-sk-64-CHARACTER-RANDOM-STRING
  description: API key for authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ahasend-openapi-v2.yaml
  type: http
- in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/ahasend-openapi.yml
  type: apiKey
slug: ahasend-authentication
source_filename: ahasend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ahasend-openapi-v2.yaml, openapi/ahasend-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: aha-sk-64-CHARACTER-RANDOM-STRING\n  description: API key for authentication\n  sources:\n  - openapi/ahasend-openapi-v2.yaml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ahasend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/authentication/ahasend-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
---
