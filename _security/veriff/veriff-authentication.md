---
api_key_in:
- header
api_specs:
- filename: veriff-openapi.yml
  format: yaml
  label: Veriff Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff/refs/heads/main/openapi/veriff-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Veriff Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veriff secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veriff
provider_slug: veriff
scheme_count: 1
schemes:
- description: Veriff requires X-AUTH-CLIENT (API key) and X-HMAC-SIGNATURE (HMAC-SHA256 of the request body using the shared secret) headers on every request.
  in: header
  name: VeriffAuth
  parameter: X-AUTH-CLIENT
  sources:
  - openapi/veriff-openapi.yml
  type: apiKey
slug: veriff-authentication
source_filename: veriff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veriff-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: VeriffAuth\n  type: apiKey\n  in: header\n  parameter: X-AUTH-CLIENT\n  description: Veriff requires X-AUTH-CLIENT (API key) and X-HMAC-SIGNATURE (HMAC-SHA256 of\n    the request body using the shared secret) headers on every request.\n  sources:\n  - openapi/veriff-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veriff/refs/heads/main/authentication/veriff-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- KYC
- Identity Verification
- Biometrics
- Fraud Prevention
- AML
- SaaS
---
