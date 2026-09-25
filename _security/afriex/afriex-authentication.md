---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: afriex-balance-api-openapi.yml
  format: yaml
  label: Afriex Balance API
  slug: afriex-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-balance-api-openapi.yml
- filename: afriex-checkout-sessions-api-openapi.yml
  format: yaml
  label: Afriex Checkout Sessions API
  slug: afriex-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-checkout-sessions-api-openapi.yml
- filename: afriex-customers-api-openapi.yml
  format: yaml
  label: Afriex Customers API
  slug: afriex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-customers-api-openapi.yml
- filename: afriex-media-api-openapi.yml
  format: yaml
  label: Afriex Media API
  slug: afriex-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-media-api-openapi.yml
- filename: afriex-payment-methods-api-openapi.yml
  format: yaml
  label: Afriex Payment Methods API
  slug: afriex-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-payment-methods-api-openapi.yml
- filename: afriex-rates-api-openapi.yml
  format: yaml
  label: Afriex Rates API
  slug: afriex-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-rates-api-openapi.yml
- filename: afriex-sme-registration-api-openapi.yml
  format: yaml
  label: Afriex SME Registration API
  slug: afriex-sme-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-sme-registration-api-openapi.yml
- filename: afriex-transactions-api-openapi.yml
  format: yaml
  label: Afriex Transactions API
  slug: afriex-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-transactions-api-openapi.yml
- filename: afriex-webhooks-api-openapi.yml
  format: yaml
  label: Afriex Webhooks API
  slug: afriex-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Afriex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Afriex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Afriex
provider_slug: afriex
scheme_count: 1
schemes:
- description: Static business API key issued from the dashboard. A business can provision **multiple API keys**, each scoped to a configurable set of **permissions** (e.g. read transactions, create deposits, etc). Permissions are chosen per key at creation time in the dashboard and may be revoked by deleting the key. Requests made with a key that does not include the permission required by the target endpoint i
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/afriex-business-openapi-original.json
  type: apiKey
slug: afriex-authentication
source_filename: afriex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: openapi/afriex-business-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Static business API key issued from the dashboard. A business can provision **multiple\n    API keys**, each scoped to a configurable set of **permissions** (e.g. read transactions,\n    create deposits, etc). Permissions are chosen per key at creation time in the dashboard\n    and may be revoked by deleting the key. Requests made with a key that does not include the\n    permission required by the target endpoint i\n  sources:\n  - openapi/afriex-business-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/authentication/afriex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Remittances
- Cross-Border Payments
- Fintech
- Financial Services
- Foreign Exchange
- Mobile Money
- Money Transfer
- Africa
- Stablecoins
- Virtual Accounts
- Webhook
- A2A
---
