---
api_key_in: []
api_specs:
- filename: hubilo-openapi.yml
  format: yaml
  label: Hubilo (Virtual PRO) Public API
  slug: hubilo-virtual-pro-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hubilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: hubilo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: hubilo
provider_slug: hubilo
scheme_count: 1
schemes:
- description: Access Token issued to the organiser, sent in the Authorization header as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hubilo-openapi.yml
  type: http
slug: hubilo-authentication
source_filename: hubilo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hubilo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access Token issued to the organiser, sent in the Authorization header as a Bearer\n    token.\n  sources:\n  - openapi/hubilo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/authentication/hubilo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Events
- Virtual Events
- Webinars
- Event Management
- Hybrid Events
- Attendee Engagement
---
