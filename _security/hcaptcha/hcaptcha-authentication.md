---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hcaptcha Authentication
name_suffix: Authentication
oauth_flows: []
overview: hCaptcha secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: hCaptcha
provider_slug: hcaptcha
scheme_count: 1
schemes:
- description: 'The hCaptcha secret key is passed as a form field named `secret` in the

    request body (application/x-www-form-urlencoded). It is modeled here as

    an apiKey scheme for tooling compatibility; the actual transport is the

    form body, not a query string.'
  in: query
  name: secretKey
  parameter: secret
  sources:
  - openapi/hcaptcha-openapi.yml
  type: apiKey
slug: hcaptcha-authentication
source_filename: hcaptcha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hcaptcha-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: secretKey\n  type: apiKey\n  in: query\n  parameter: secret\n  description: |-\n    The hCaptcha secret key is passed as a form field named `secret` in the\n    request body (application/x-www-form-urlencoded). It is modeled here as\n    an apiKey scheme for tooling compatibility; the actual transport is the\n    form body, not a query string.\n  sources:\n  - openapi/hcaptcha-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcaptcha/refs/heads/main/authentication/hcaptcha-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CAPTCHA
- Bot Defense
- Privacy
- hCaptcha
- Intuition Machines
- Account Defense
- Enterprise Security
---
