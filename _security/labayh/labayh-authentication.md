---
api_key_in:
- header
api_specs:
- filename: labayh-content-openapi.yml
  format: yaml
  label: Labayh Content API
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labayh/refs/heads/main/openapi/labayh-content-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Labayh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Labayh secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Labayh
provider_slug: labayh
scheme_count: 2
schemes:
- description: 'WordPress application passwords, advertised by the API index at https://labayh.net/wp-json/ (authorization endpoint: https://labayh.net/wp-admin/authorize-application.php). Required for every write operation; the documented read operations need no credentials.'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/labayh-content-openapi.yml
  type: http
- description: Cookie-authenticated first-party requests pass a nonce in the X-WP-Nonce header.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/labayh-content-openapi.yml
  type: apiKey
slug: labayh-authentication
source_filename: labayh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/labayh-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress application passwords, advertised by the API index at https://labayh.net/wp-json/\n    (authorization endpoint: https://labayh.net/wp-admin/authorize-application.php). Required\n    for every write operation; the documented read operations need no credentials.'\n  sources:\n  - openapi/labayh-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: Cookie-authenticated first-party requests pass a nonce in the X-WP-Nonce header.\n  sources:\n  - openapi/labayh-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labayh/refs/heads/main/authentication/labayh-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Mental Health
- Healthcare
- Telehealth
- Therapy
- Wellbeing
- Content
- Saudi Arabia
- Middle East
- Arabic
---
