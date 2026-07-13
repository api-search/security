---
api_key_in:
- cookie
api_specs:
- filename: lenovo-openapi.yml
  format: yaml
  label: Lenovo XClarity Administrator REST API
  slug: lenovo-xclarity-administrator-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lenovo/refs/heads/main/openapi/lenovo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lenovo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lenovo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lenovo
provider_slug: lenovo
scheme_count: 1
schemes:
- description: 'Session cookie issued by `POST /sessions`. Requests also require

    the `X-Csrf-Token` header populated from the session response.'
  in: cookie
  name: sessionCookie
  parameter: JSESSIONID
  sources:
  - openapi/lenovo-openapi.yml
  type: apiKey
slug: lenovo-authentication
source_filename: lenovo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lenovo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: |-\n    Session cookie issued by `POST /sessions`. Requests also require\n    the `X-Csrf-Token` header populated from the session response.\n  sources:\n  - openapi/lenovo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lenovo/refs/heads/main/authentication/lenovo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Center
- Hardware
- Infrastructure
- Personal Computers
- Servers
- Technology
---
