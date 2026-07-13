---
api_key_in:
- cookie
api_specs:
- filename: docs
  format: yaml
  label: GlitchTip REST API
  slug: glitchtip-rest-api
  spec_type: OpenAPI
  url: https://app.glitchtip.com/api/docs
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Glitchtip Authentication
name_suffix: Authentication
oauth_flows: []
overview: GlitchTip secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GlitchTip
provider_slug: glitchtip
scheme_count: 2
schemes:
- name: TokenAuth
  scheme: bearer
  sources:
  - openapi/glitchtip-rest-openapi.yml
  type: http
- in: cookie
  name: SessionAuth
  parameter: sessionid
  sources:
  - openapi/glitchtip-rest-openapi.yml
  type: apiKey
slug: glitchtip-authentication
source_filename: glitchtip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glitchtip-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/glitchtip-rest-openapi.yml\n- name: SessionAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/glitchtip-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/authentication/glitchtip-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Error Tracking
- Performance Monitoring
- Uptime Monitoring
- Application Monitoring
- Open Source
- Sentry Compatible
- Observability
- Logging
---
