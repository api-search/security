---
api_key_in:
- header
api_specs:
- filename: modulr-api.json
  format: json
  label: Modulr Accounts API
  slug: modulr-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Payments API
  slug: modulr-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Cards API
  slug: modulr-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Direct Debits API
  slug: modulr-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Customers API
  slug: modulr-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Payee Verification API
  slug: modulr-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Payment Initiation API
  slug: modulr-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Variable Recurring Payments API
  slug: modulr-variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Notifications API
  slug: modulr-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Modulr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modulr secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Modulr
provider_slug: modulr
scheme_count: 2
schemes:
- in: header
  name: modulo_security
  parameter: Authorization
  sources:
  - openapi/modulr-api.json
  type: apiKey
- in: header
  name: TOKEN
  note: Sandbox-only bearer token shortcut. Uses the base URL https://api-sandbox.modulrfinance.com/api-sandbox-token/ and the raw API Key as the Authorization value. Not accepted in production.
  parameter: Authorization
  sources:
  - openapi/modulr-api.json
  type: apiKey
slug: modulr-authentication
source_filename: modulr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/modulr-api.json\ndocs: https://modulr.readme.io/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: HMAC request signing (draft HTTP Signatures) over an API Key + HMAC secret\nschemes:\n- name: modulo_security\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/modulr-api.json\n- name: TOKEN\n  type: apiKey\n  in: header\n  parameter: Authorization\n  note: >-\n    Sandbox-only bearer token shortcut. Uses the base URL\n    https://api-sandbox.modulrfinance.com/api-sandbox-token/ and the raw API Key\n    as the Authorization value. Not accepted in production.\n  sources:\n  - openapi/modulr-api.json\ndetails:\n  production_auth: HMAC\n  hmac:\n    standard: HMAC HTTP request signing (latest draft of the HMAC request-signing standard)\n    algorithm: hmac-sha1\n    signed_headers:\n    - date\n    - x-mod-nonce\n    authorization_format: >-\n      Signature\
  \ keyId=\"<API_KEY>\",algorithm=\"hmac-sha1\",headers=\"date x-mod-nonce\",signature=\"<url-encoded-base64>\"\n    credentials:\n    - API Key (aka token)\n    - API HMAC Secret (aka hmac/secret)\n    required_headers:\n    - name: Date\n      note: RFC 7231 HTTP-date, GMT (e.g. \"Mon, 25 Jul 2016 16:36:07 GMT\")\n    - name: x-mod-nonce\n      note: unique value per request; reused only for idempotent retries\n    - name: Authorization\n      note: the Signature header\n    clock_skew: enforced (recommended NTP sync) to prevent replay attacks\n  ip_allowlisting: Production API access is restricted by IP address (allowlist requested at onboarding)\n  transport: HTTPS required in all environments\n  sample_code: https://github.com/Modulr-finance/modulr-hmac\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/authentication/modulr-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- United Kingdom
- Banking-as-a-Service
- Embedded Finance
- Payment Processing
- Account-to-Account
- Open Banking
- Faster Payments
- Card Issuing
- Direct Debit
- Confirmation of Payee
- Variable Recurring Payments
---
