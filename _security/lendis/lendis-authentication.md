---
api_key_in:
- header
api_specs:
- filename: lendis-content-openapi.yml
  format: yaml
  label: Lendis Content API (WordPress REST)
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendis/refs/heads/main/openapi/lendis-content-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lendis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lendis secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lendis
provider_slug: lendis
scheme_count: 2
schemes:
- description: WordPress Application Passwords (username plus application password) sent as HTTP Basic over TLS. Required for write operations and privileged routes; anonymous read access needs no credentials.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/lendis-content-openapi.yml
  type: http
- description: Cookie-authenticated first-party browser requests send a WordPress nonce in the X-WP-Nonce header, advertised in Access-Control-Allow-Headers on live responses.
  in: header
  name: nonce
  parameter: X-WP-Nonce
  sources:
  - openapi/lendis-content-openapi.yml
  type: apiKey
slug: lendis-authentication
source_filename: lendis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lendis-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (username plus application password) sent as\n    HTTP Basic over TLS. Required for write operations and privileged routes; anonymous read\n    access needs no credentials.\n  sources:\n  - openapi/lendis-content-openapi.yml\n- name: nonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: Cookie-authenticated first-party browser requests send a WordPress nonce in the\n    X-WP-Nonce header, advertised in Access-Control-Allow-Headers on live responses.\n  sources:\n  - openapi/lendis-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendis/refs/heads/main/authentication/lendis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai Enterprise Software
- Device As A Service
- IT Hardware
- Leasing
- Asset Management
- Workplace Technology
- Procurement
- Germany
- SaaS
---
