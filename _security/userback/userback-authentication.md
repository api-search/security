---
api_key_in: []
api_specs:
- filename: userback-openapi.yml
  format: yaml
  label: Userback REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userback/refs/heads/main/openapi/userback-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Userback Authentication
name_suffix: Authentication
oauth_flows: []
overview: Userback secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Userback
provider_slug: userback
scheme_count: 1
schemes:
- bearerFormat: API Token
  description: Pass the Userback API token in the Authorization header as `Bearer <YOUR_API_TOKEN>`. Tokens are managed from the Userback dashboard.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/userback-openapi.yml
  type: http
slug: userback-authentication
source_filename: userback-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/userback-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  description: Pass the Userback API token in the Authorization header as `Bearer <YOUR_API_TOKEN>`.\n    Tokens are managed from the Userback dashboard.\n  sources:\n  - openapi/userback-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userback/refs/heads/main/authentication/userback-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Feedback
- Bug Reporting
- Visual Feedback
- Session Replay
- Product Management
- SaaS
---
