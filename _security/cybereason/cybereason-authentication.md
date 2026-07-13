---
api_key_in:
- cookie
api_specs:
- filename: cybereason-openapi.yml
  format: yaml
  label: Cybereason REST API
  slug: cybereason-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cybereason Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cybereason secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cybereason
provider_slug: cybereason
scheme_count: 2
schemes:
- description: Session cookie returned by POST /login.html.
  in: cookie
  name: SessionCookie
  parameter: JSESSIONID
  sources:
  - openapi/cybereason-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Available on Cybereason 20.1+ for token-based access.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cybereason-openapi.yml
  type: http
slug: cybereason-authentication
source_filename: cybereason-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cybereason-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: Session cookie returned by POST /login.html.\n  sources:\n  - openapi/cybereason-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Available on Cybereason 20.1+ for token-based access.\n  sources:\n  - openapi/cybereason-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/authentication/cybereason-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cybersecurity
- XDR
- EDR
- NGAV
- MDR
- Endpoint Security
- Threat Detection
---
