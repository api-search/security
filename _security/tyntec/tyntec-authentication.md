---
api_key_in: []
api_specs:
- filename: tyntec-number-verification-openapi.yml
  format: yaml
  label: tyntec Number Verification API
  slug: tyntec-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/openapi/tyntec-number-verification-openapi.yml
- filename: tyntec-number-verification-openapi.yml
  format: yaml
  label: tyntec Number Information API
  slug: tyntec-number-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/openapi/tyntec-number-verification-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tyntec Authentication
name_suffix: Authentication
oauth_flows: []
overview: tyntec secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: tyntec
provider_slug: tyntec
scheme_count: 1
schemes:
- description: All tyntec APIs (Verify / Number Information, SMS, Conversations / WhatsApp, and 2FA) authenticate with an account API key created in the tyntec Console and sent in the `apikey` request header on every call. The Verify API reference documents the same key as `apiKey`; the header is case-insensitive. There is no OAuth or Bearer flow on tyntec's public REST APIs.
  in: header
  name: apiKeyAuth
  parameterName: apikey
  sources:
  - openapi/tyntec-number-verification-openapi.yml
  - https://api.tyntec.com/reference/verify/current.html
  - https://api.tyntec.com/reference/sms/current.html
  - https://api.tyntec.com/reference/conversations/current.html
  type: apiKey
slug: tyntec-authentication
source_filename: tyntec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tyntec-number-verification-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: apikey\n  description: >-\n    All tyntec APIs (Verify / Number Information, SMS, Conversations / WhatsApp,\n    and 2FA) authenticate with an account API key created in the tyntec Console\n    and sent in the `apikey` request header on every call. The Verify API\n    reference documents the same key as `apiKey`; the header is case-insensitive.\n    There is no OAuth or Bearer flow on tyntec's public REST APIs.\n  sources:\n  - openapi/tyntec-number-verification-openapi.yml\n  - https://api.tyntec.com/reference/verify/current.html\n  - https://api.tyntec.com/reference/sms/current.html\n  - https://api.tyntec.com/reference/conversations/current.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/authentication/tyntec-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Number Verification
- CPaaS
- SMS
- WhatsApp
- Phone Number Intelligence
- HLR Lookup
- Two-Factor Authentication
- OTP
- Messaging
- Number Portability
---
