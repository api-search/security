---
api_key_in: []
api_specs:
- filename: hacware-openapi.yml
  format: yaml
  label: HacWare Security Awareness API
  slug: hacware-security-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hacware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hacware secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hacware
provider_slug: hacware
scheme_count: 1
schemes:
- description: Bearer access token obtained from POST /api/v1/auth/ (exchange appid + secret key). Tokens expire ~1 hour after issue; use the refresh token to renew.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hacware-openapi.yml
  type: http
slug: hacware-authentication
source_filename: hacware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hacware-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained from POST /api/v1/auth/ (exchange appid + secret\n    key). Tokens expire ~1 hour after issue; use the refresh token to renew.\n  sources:\n  - openapi/hacware-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/authentication/hacware-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Security Awareness
- Phishing
- Training
- Compliance
- Email Security
- Artificial Intelligence
---
