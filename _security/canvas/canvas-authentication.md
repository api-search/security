---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Canvas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canvas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Canvas
provider_slug: canvas
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 access token. See

    https://canvas.instructure.com/doc/api/file.oauth.html.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/canvas-openapi.yml
  type: http
slug: canvas-authentication
source_filename: canvas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canvas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token. See\n    https://canvas.instructure.com/doc/api/file.oauth.html.\n  sources:\n  - openapi/canvas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/authentication/canvas-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- EdTech
- GraphQL
- Learning Management System
- LMS
- LTI
- Open Source
- REST
---
