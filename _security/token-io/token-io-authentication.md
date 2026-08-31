---
api_key_in:
- header
api_specs:
- filename: token-io-account-on-file-api-openapi.yml
  format: yaml
  label: token-io Account on File API
  slug: token-io-account-on-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-account-on-file-api-openapi.yml
- filename: token-io-accounts-api-openapi.yml
  format: yaml
  label: token-io Accounts API
  slug: token-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-accounts-api-openapi.yml
- filename: token-io-authentication-keys-api-openapi.yml
  format: yaml
  label: token-io Authentication keys API
  slug: token-io-authentication-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-authentication-keys-api-openapi.yml
- filename: token-io-banks-v1-api-openapi.yml
  format: yaml
  label: token-io Banks v1 API
  slug: token-io-banks-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-banks-v1-api-openapi.yml
- filename: token-io-banks-v2-api-openapi.yml
  format: yaml
  label: token-io Banks v2 API
  slug: token-io-banks-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-banks-v2-api-openapi.yml
- filename: token-io-pay-by-link-api-openapi.yml
  format: yaml
  label: token-io Pay by Link API
  slug: token-io-pay-by-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-pay-by-link-api-openapi.yml
- filename: token-io-payments-v2-api-openapi.yml
  format: yaml
  label: token-io Payments v2 API
  slug: token-io-payments-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-payments-v2-api-openapi.yml
- filename: token-io-payouts-api-openapi.yml
  format: yaml
  label: token-io Payouts API
  slug: token-io-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-payouts-api-openapi.yml
- filename: token-io-refunds-api-openapi.yml
  format: yaml
  label: token-io Refunds API
  slug: token-io-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-refunds-api-openapi.yml
- filename: token-io-reports-api-openapi.yml
  format: yaml
  label: token-io Reports API
  slug: token-io-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-reports-api-openapi.yml
- filename: token-io-requests-for-payments-v1-or-ais-api-openapi.yml
  format: yaml
  label: token-io Requests - for Payments v1 or AIS API
  slug: token-io-requests-for-payments-v1-or-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-requests-for-payments-v1-or-ais-api-openapi.yml
- filename: token-io-settlement-accounts-api-openapi.yml
  format: yaml
  label: token-io Settlement Accounts API
  slug: token-io-settlement-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-settlement-accounts-api-openapi.yml
- filename: token-io-sub-tpps-api-openapi.yml
  format: yaml
  label: token-io Sub-TPPs API
  slug: token-io-sub-tpps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-sub-tpps-api-openapi.yml
- filename: token-io-tokens-api-openapi.yml
  format: yaml
  label: token-io Tokens API
  slug: token-io-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-tokens-api-openapi.yml
- filename: token-io-transfers-for-payments-v1-api-openapi.yml
  format: yaml
  label: token-io Transfers - for Payments v1 API
  slug: token-io-transfers-for-payments-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-transfers-for-payments-v1-api-openapi.yml
- filename: token-io-variable-recurring-payments-api-openapi.yml
  format: yaml
  label: token-io Variable Recurring Payments API
  slug: token-io-variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-variable-recurring-payments-api-openapi.yml
- filename: token-io-verification-api-openapi.yml
  format: yaml
  label: token-io Verification API
  slug: token-io-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-verification-api-openapi.yml
- filename: token-io-webhooks-api-openapi.yml
  format: yaml
  label: token-io Webhooks API
  slug: token-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Token Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Token.io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Token.io
provider_slug: token-io
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: '**For Production and Sandbox environments.**<br />When using curl samples the authorization header is given as -H `''Authorization: Bearer + JWT''`<br/>Please substitute your Bearer key here.<br/>For example:<br/> -H `''Authorization: Bearer [example key]'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/token-io-openapi.yml
  type: http
- description: '**For Sandbox environment only.**<br />When using curl samples the authorization header is given as -H `''Authorization: YOUR_API_KEY_HERE''`<br/>Please substitute your Basic key here.<br/>For example:<br/> -H `''Authorization: Basic [example key]''`'
  in: header
  name: BasicAuth
  parameter: Authorization
  sources:
  - openapi/token-io-openapi.yml
  type: apiKey
slug: token-io-authentication
source_filename: token-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/token-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: '**For Production and Sandbox environments.**<br />When using curl samples the\n    authorization header is given as -H `''Authorization: Bearer + JWT''`<br/>Please substitute\n    your Bearer key here.<br/>For example:<br/> -H `''Authorization: Bearer [example key]'\n  sources:\n  - openapi/token-io-openapi.yml\n- name: BasicAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '**For Sandbox environment only.**<br />When using curl samples the authorization\n    header is given as -H `''Authorization: YOUR_API_KEY_HERE''`<br/>Please substitute your\n    Basic key here.<br/>For example:<br/> -H `''Authorization: Basic [example key]''`'\n  sources:\n  - openapi/token-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/authentication/token-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
