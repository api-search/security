---
api_key_in: []
api_specs:
- filename: qiwi-openapi.yml
  format: yaml
  label: Qiwi Payment Protocol
  slug: qiwi-payment-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qiwi/refs/heads/main/openapi/qiwi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qiwi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qiwi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qiwi
provider_slug: qiwi
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qiwi-openapi.yml
  type: http
slug: qiwi-authentication
source_filename: qiwi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qiwi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/qiwi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qiwi/refs/heads/main/authentication/qiwi-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Wallet
- Payouts
- Fintech
- Banking
---
