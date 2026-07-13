---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: dLocal Payins API
  slug: dlocal-payins-api
  spec_type: OpenAPI
  url: https://docs.dlocal.com/llms.txt
- filename: dlocal-payouts-openapi.yml
  format: yaml
  label: dLocal Payouts API
  slug: dlocal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payouts-openapi.yml
- filename: dlocal-platforms-openapi.yml
  format: yaml
  label: dLocal Platforms API
  slug: dlocal-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-platforms-openapi.yml
- filename: dlocal-verification-openapi.yml
  format: yaml
  label: dLocal Verification API
  slug: dlocal-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-verification-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dlocal Authentication
name_suffix: Authentication
oauth_flows: []
overview: dLocal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dLocal
provider_slug: dlocal
scheme_count: 1
schemes:
- description: 'HMAC-SHA256 signature. Format: "V2-HMAC-SHA256, Signature: {hmac_value}" Signature = HMAC-SHA256(X-Login + X-Date + RequestBody, SecretKey)'
  in: header
  name: HmacAuth
  parameter: Authorization
  sources:
  - openapi/dlocal-payins-openapi.yml
  - openapi/dlocal-payouts-openapi.yml
  - openapi/dlocal-platforms-openapi.yml
  - openapi/dlocal-verification-openapi.yml
  type: apiKey
slug: dlocal-authentication
source_filename: dlocal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dlocal-payins-openapi.yml, openapi/dlocal-payouts-openapi.yml, openapi/dlocal-platforms-openapi.yml,\n  openapi/dlocal-verification-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'HMAC-SHA256 signature. Format: \"V2-HMAC-SHA256, Signature: {hmac_value}\" Signature\n    = HMAC-SHA256(X-Login + X-Date + RequestBody, SecretKey)'\n  sources:\n  - openapi/dlocal-payins-openapi.yml\n  - openapi/dlocal-payouts-openapi.yml\n  - openapi/dlocal-platforms-openapi.yml\n  - openapi/dlocal-verification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/authentication/dlocal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Emerging Markets
- Payins
- Payouts
- Fintech
- Latin America
- Africa
- Asia
- Local Payment Methods
- Payment Processing
---
