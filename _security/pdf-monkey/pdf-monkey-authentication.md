---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: PDF Monkey API
  slug: pdf-monkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pdf Monkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: PDF Monkey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PDF Monkey
provider_slug: pdf-monkey
scheme_count: 1
schemes:
- description: Authenticate using your PDF Monkey API secret key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: pdf-monkey-authentication
source_filename: pdf-monkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate using your PDF Monkey API secret key as a Bearer token in the Authorization\n    header.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/authentication/pdf-monkey-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- Document Generation
- Templates
- Handlebars
- REST API
- Webhooks
---
