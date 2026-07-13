---
api_key_in: []
api_specs:
- filename: umami-openapi.yml
  format: yaml
  label: Umami API
  slug: umami-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Umami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Umami secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Umami
provider_slug: umami
scheme_count: 1
schemes:
- description: JWT token obtained from POST /api/auth/login or Umami Cloud API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/umami-openapi.yml
  type: http
slug: umami-authentication
source_filename: umami-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/umami-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT token obtained from POST /api/auth/login or Umami Cloud API key\n  sources:\n  - openapi/umami-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/authentication/umami-authentication.yml
summary_line: http · 1 scheme
tags:
- Cookieless Tracking
- Open Source
- Privacy
- Web Analytics
- Website Analytics
---
