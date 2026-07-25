---
api_key_in: []
api_specs:
- filename: xflow-accounts-api-openapi.yml
  format: yaml
  label: Xflow Accounts API
  slug: xflow-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-accounts-api-openapi.yml
- filename: xflow-accountsettings-api-openapi.yml
  format: yaml
  label: Xflow AccountSettings API
  slug: xflow-accountsettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-accountsettings-api-openapi.yml
- filename: xflow-addresses-api-openapi.yml
  format: yaml
  label: Xflow Addresses API
  slug: xflow-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-addresses-api-openapi.yml
- filename: xflow-balance-api-openapi.yml
  format: yaml
  label: Xflow Balance API
  slug: xflow-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-balance-api-openapi.yml
- filename: xflow-balancetransactions-api-openapi.yml
  format: yaml
  label: Xflow BalanceTransactions API
  slug: xflow-balancetransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-balancetransactions-api-openapi.yml
- filename: xflow-deposits-api-openapi.yml
  format: yaml
  label: Xflow Deposits API
  slug: xflow-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-deposits-api-openapi.yml
- filename: xflow-events-api-openapi.yml
  format: yaml
  label: Xflow Events API
  slug: xflow-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-events-api-openapi.yml
- filename: xflow-exchangerates-api-openapi.yml
  format: yaml
  label: Xflow ExchangeRates API
  slug: xflow-exchangerates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-exchangerates-api-openapi.yml
- filename: xflow-feeplans-api-openapi.yml
  format: yaml
  label: Xflow FeePlans API
  slug: xflow-feeplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-feeplans-api-openapi.yml
- filename: xflow-files-api-openapi.yml
  format: yaml
  label: Xflow Files API
  slug: xflow-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-files-api-openapi.yml
- filename: xflow-paymentlinks-api-openapi.yml
  format: yaml
  label: Xflow PaymentLinks API
  slug: xflow-paymentlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-paymentlinks-api-openapi.yml
- filename: xflow-payments-api-openapi.yml
  format: yaml
  label: Xflow Payments API
  slug: xflow-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-payments-api-openapi.yml
- filename: xflow-payouts-api-openapi.yml
  format: yaml
  label: Xflow Payouts API
  slug: xflow-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-payouts-api-openapi.yml
- filename: xflow-persons-api-openapi.yml
  format: yaml
  label: Xflow Persons API
  slug: xflow-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-persons-api-openapi.yml
- filename: xflow-quotes-api-openapi.yml
  format: yaml
  label: Xflow Quotes API
  slug: xflow-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-quotes-api-openapi.yml
- filename: xflow-receivables-api-openapi.yml
  format: yaml
  label: Xflow Receivables API
  slug: xflow-receivables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-receivables-api-openapi.yml
- filename: xflow-transfers-api-openapi.yml
  format: yaml
  label: Xflow Transfers API
  slug: xflow-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-transfers-api-openapi.yml
- filename: xflow-webhookendpoints-api-openapi.yml
  format: yaml
  label: Xflow WebhookEndpoints API
  slug: xflow-webhookendpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-webhookendpoints-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Xflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xflow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xflow
provider_slug: xflow
scheme_count: 1
schemes:
- bearerFormat: auth-scheme
  description: 'Bearer HTTP authentication. Allowed headers-- Authorization: Bearer <api_key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/xflow-openapi-original.yml
  type: http
slug: xflow-authentication
source_filename: xflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/xflow-openapi-original.yml\ndocs: https://docs.xflowpay.com/latest/api\nsummary:\n  types:\n  - http\n  styles:\n  - bearer\n  - basic (API key as username, empty password)\n  key_prefixes:\n    test: sk_test_\n    live: sk_live_\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: auth-scheme\n  description: 'Bearer HTTP authentication. Allowed headers-- Authorization: Bearer <api_key>'\n  sources:\n  - openapi/xflow-openapi-original.yml\nnotes: API keys are managed in the Xflow dashboard. Test keys are prefixed sk_test_\n  and live keys sk_live_; testmode and livemode data are fully separate. The docs\n  also allow supplying the API key as the HTTP Basic auth username with no\n  password. All requests must use HTTPS; plain HTTP calls fail. Platforms act on\n  behalf of connected users with the Xflow-Account header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/authentication/xflow-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Cross-Border Payments
- Fintech
- India
- Foreign Exchange
- Invoicing
- Payouts
---
