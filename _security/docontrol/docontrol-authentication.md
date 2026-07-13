---
api_key_in: []
api_specs:
- filename: docontrol-openapi.yml
  format: yaml
  label: DoControl
  slug: docontrol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/openapi/docontrol-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docontrol Authentication
name_suffix: Authentication
oauth_flows: []
overview: DoControl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DoControl
provider_slug: docontrol
scheme_count: 1
schemes:
- description: Access token returned from /refresh
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/docontrol-openapi.yml
  type: http
slug: docontrol-authentication
source_filename: docontrol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docontrol-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token returned from /refresh\n  sources:\n  - openapi/docontrol-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/authentication/docontrol-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Security
- SaaS Security
---
