---
api_key_in:
- header
api_specs:
- filename: cryptomus-recurring-payments-api-openapi.yml
  format: yaml
  label: Cryptomus Recurring Payments API
  slug: cryptomus-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-recurring-payments-api-openapi.yml
- filename: cryptomus-exchange-api-openapi.yml
  format: yaml
  label: Cryptomus Exchange API
  slug: cryptomus-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-exchange-api-openapi.yml
- filename: cryptomus-payments-api-openapi.yml
  format: yaml
  label: Cryptomus Payments API
  slug: cryptomus-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-payments-api-openapi.yml
- filename: cryptomus-payouts-api-openapi.yml
  format: yaml
  label: Cryptomus Payouts API
  slug: cryptomus-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-payouts-api-openapi.yml
- filename: cryptomus-recurring-payments-api-openapi.yml
  format: yaml
  label: Cryptomus Recurring Payments API
  slug: cryptomus-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-recurring-payments-api-openapi.yml
- filename: cryptomus-wallets-api-openapi.yml
  format: yaml
  label: Cryptomus Wallets API
  slug: cryptomus-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-wallets-api-openapi.yml
- filename: cryptomus-webhooks-api-openapi.yml
  format: yaml
  label: Cryptomus Webhooks API
  slug: cryptomus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/cryptomus-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cryptomus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cryptomus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cryptomus
provider_slug: cryptomus
scheme_count: 1
schemes:
- description: Merchant UUID from personal account settings. All requests also require a `sign` header computed as MD5(base64_encode(request_body) + API_KEY).
  in: header
  name: MerchantAuth
  parameter: merchant
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: cryptomus-authentication
source_filename: cryptomus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: MerchantAuth\n  type: apiKey\n  in: header\n  parameter: merchant\n  description: Merchant UUID from personal account settings. All requests also require a `sign`\n    header computed as MD5(base64_encode(request_body) + API_KEY).\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/authentication/cryptomus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Payments
- Invoices
- Payouts
- Exchange Rates
- Crypto Gateway
---
