---
api_key_in:
- header
api_specs:
- filename: aza-finance-account-debits-api-openapi.yml
  format: yaml
  label: AZA Finance Account Debits API
  slug: aza-finance-account-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-account-debits-api-openapi.yml
- filename: aza-finance-account-validation-api-openapi.yml
  format: yaml
  label: AZA Finance Account Validation API
  slug: aza-finance-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-account-validation-api-openapi.yml
- filename: aza-finance-accounts-api-openapi.yml
  format: yaml
  label: AZA Finance Accounts API
  slug: aza-finance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-accounts-api-openapi.yml
- filename: aza-finance-api-logs-api-openapi.yml
  format: yaml
  label: AZA Finance API Logs API
  slug: aza-finance-api-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-api-logs-api-openapi.yml
- filename: aza-finance-currency-info-api-openapi.yml
  format: yaml
  label: AZA Finance Currency Info API
  slug: aza-finance-currency-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-currency-info-api-openapi.yml
- filename: aza-finance-dlocal-balance-api-openapi.yml
  format: yaml
  label: AZA Finance dlocal balance API
  slug: aza-finance-dlocal-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-dlocal-balance-api-openapi.yml
- filename: aza-finance-documents-api-openapi.yml
  format: yaml
  label: AZA Finance Documents API
  slug: aza-finance-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-documents-api-openapi.yml
- filename: aza-finance-logs-api-openapi.yml
  format: yaml
  label: AZA Finance Logs API
  slug: aza-finance-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-logs-api-openapi.yml
- filename: aza-finance-mandates-api-openapi.yml
  format: yaml
  label: AZA Finance Mandates API
  slug: aza-finance-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-mandates-api-openapi.yml
- filename: aza-finance-payin-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payin Methods API
  slug: aza-finance-payin-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payin-methods-api-openapi.yml
- filename: aza-finance-payment-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payment Methods API
  slug: aza-finance-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payment-methods-api-openapi.yml
- filename: aza-finance-payout-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payout Methods API
  slug: aza-finance-payout-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payout-methods-api-openapi.yml
- filename: aza-finance-recipients-api-openapi.yml
  format: yaml
  label: AZA Finance Recipients API
  slug: aza-finance-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-recipients-api-openapi.yml
- filename: aza-finance-senders-api-openapi.yml
  format: yaml
  label: AZA Finance Senders API
  slug: aza-finance-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-senders-api-openapi.yml
- filename: aza-finance-transactions-api-openapi.yml
  format: yaml
  label: AZA Finance Transactions API
  slug: aza-finance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-transactions-api-openapi.yml
- filename: aza-finance-webhooks-api-openapi.yml
  format: yaml
  label: AZA Finance Webhooks API
  slug: aza-finance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aza Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: AZA Finance secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AZA Finance
provider_slug: aza-finance
scheme_count: 4
schemes:
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationKey
  parameter: Authorization-Key
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationSecret
  parameter: Authorization-Secret
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationNonce
  parameter: Authorization-Nonce
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationSignature
  parameter: Authorization-Signature
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
slug: aza-finance-authentication
source_filename: aza-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/aza-finance-openapi-original.json\ndocs: https://docs.transferzero.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: hmac\n  detail: >-\n    Two documented modes. Preferred: HMAC request signing using Authorization-Key,\n    Authorization-Nonce and Authorization-Signature headers (signature is an HMAC over\n    the request built from the API secret). Simpler alternative for lower-risk calls:\n    Authorization-Key + Authorization-Secret. Sandbox and production use separate\n    key/secret pairs. Webhook callbacks are signed with the same HMAC scheme.\nschemes:\n- name: AuthorizationKey\n  type: apiKey\n  in: header\n  parameter: Authorization-Key\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n- name: AuthorizationSecret\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization-Secret\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n- name: AuthorizationNonce\n  type: apiKey\n  in: header\n  parameter: Authorization-Nonce\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n- name: AuthorizationSignature\n  type: apiKey\n  in: header\n  parameter: Authorization-Signature\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/authentication/aza-finance-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Financial-Services
- Payments
- Foreign Exchange
- Cross-Border Payments
- Africa
- Fintech
---
