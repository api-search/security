---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coingate-conversions-api-openapi.yml
  format: yaml
  label: CoinGate Conversions API
  slug: coingate-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-conversions-api-openapi.yml
- filename: coingate-currencies-api-openapi.yml
  format: yaml
  label: CoinGate Currencies API
  slug: coingate-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-currencies-api-openapi.yml
- filename: coingate-orders-api-openapi.yml
  format: yaml
  label: CoinGate Orders API
  slug: coingate-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-orders-api-openapi.yml
- filename: coingate-refunds-api-openapi.yml
  format: yaml
  label: CoinGate Refunds API
  slug: coingate-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-refunds-api-openapi.yml
- filename: coingate-send-requests-api-openapi.yml
  format: yaml
  label: CoinGate Send Requests API
  slug: coingate-send-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-send-requests-api-openapi.yml
- filename: coingate-beneficiaries-api-openapi.yml
  format: yaml
  label: CoinGate Beneficiaries API
  slug: coingate-beneficiaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-beneficiaries-api-openapi.yml
- filename: coingate-beneficiary-payout-settings-api-openapi.yml
  format: yaml
  label: CoinGate Beneficiary Payout Settings API
  slug: coingate-beneficiary-payout-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-beneficiary-payout-settings-api-openapi.yml
- filename: coingate-billing-api-openapi.yml
  format: yaml
  label: CoinGate Billing API
  slug: coingate-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-billing-api-openapi.yml
- filename: coingate-contacts-api-openapi.yml
  format: yaml
  label: CoinGate Contacts API
  slug: coingate-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-contacts-api-openapi.yml
- filename: coingate-countries-api-openapi.yml
  format: yaml
  label: CoinGate Countries API
  slug: coingate-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-countries-api-openapi.yml
- filename: coingate-deposits-api-openapi.yml
  format: yaml
  label: CoinGate Deposits API
  slug: coingate-deposits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-deposits-api-openapi.yml
- filename: coingate-industries-api-openapi.yml
  format: yaml
  label: CoinGate Industries API
  slug: coingate-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-industries-api-openapi.yml
- filename: coingate-invoice-api-openapi.yml
  format: yaml
  label: CoinGate Invoice API
  slug: coingate-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-invoice-api-openapi.yml
- filename: coingate-ledger-api-openapi.yml
  format: yaml
  label: CoinGate Ledger API
  slug: coingate-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-ledger-api-openapi.yml
- filename: coingate-mass-payouts-api-openapi.yml
  format: yaml
  label: CoinGate Mass Payouts API
  slug: coingate-mass-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-mass-payouts-api-openapi.yml
- filename: coingate-new-endpoint-api-openapi.yml
  format: yaml
  label: CoinGate New Endpoint API
  slug: coingate-new-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-new-endpoint-api-openapi.yml
- filename: coingate-payment-channels-api-openapi.yml
  format: yaml
  label: CoinGate Payment Channels API
  slug: coingate-payment-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-payment-channels-api-openapi.yml
- filename: coingate-payout-links-api-openapi.yml
  format: yaml
  label: CoinGate Payout Links API
  slug: coingate-payout-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-payout-links-api-openapi.yml
- filename: coingate-ping-api-openapi.yml
  format: yaml
  label: CoinGate Ping API
  slug: coingate-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-ping-api-openapi.yml
- filename: coingate-platforms-api-openapi.yml
  format: yaml
  label: CoinGate Platforms API
  slug: coingate-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-platforms-api-openapi.yml
- filename: coingate-rates-api-openapi.yml
  format: yaml
  label: CoinGate Rates API
  slug: coingate-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-rates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Coingate Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinGate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoinGate
provider_slug: coingate
scheme_count: 1
schemes:
- description: API Token authentication. Obtain your API token from the CoinGate merchant dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: coingate-authentication
source_filename: coingate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API Token authentication. Obtain your API token from the CoinGate merchant dashboard.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/coingate/authentication/coingate-authentication.yml
summary_line: http · 1 scheme
tags:
- Cryptocurrency
- Payments
- Payment Gateway
- Fintech
- Bitcoin
- Ethereum
- Merchant Services
---
