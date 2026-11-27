---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orsunpay-com-cashier-embedding-policy-api-openapi.yml
  format: yaml
  label: Orsun Pay Cashier embedding policy API
  slug: orsunpay-com-cashier-embedding-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-cashier-embedding-policy-api-openapi.yml
- filename: orsunpay-com-cashier-player-api-openapi.yml
  format: yaml
  label: Orsun Pay Cashier player API
  slug: orsunpay-com-cashier-player-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-cashier-player-api-openapi.yml
- filename: orsunpay-com-cashier-sessions-merchant-s2s-api-openapi.yml
  format: yaml
  label: Orsun Pay Cashier sessions (merchant S2S) API
  slug: orsunpay-com-cashier-sessions-merchant-s2s-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-cashier-sessions-merchant-s2s-api-openapi.yml
- filename: orsunpay-com-payment-links-api-openapi.yml
  format: yaml
  label: Orsun Pay Payment links API
  slug: orsunpay-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-payment-links-api-openapi.yml
- filename: orsunpay-com-payments-api-openapi.yml
  format: yaml
  label: Orsun Pay Payments API
  slug: orsunpay-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-payments-api-openapi.yml
- filename: orsunpay-com-refunds-api-openapi.yml
  format: yaml
  label: Orsun Pay Refunds API
  slug: orsunpay-com-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-refunds-api-openapi.yml
- filename: orsunpay-com-transactions-api-openapi.yml
  format: yaml
  label: Orsun Pay Transactions API
  slug: orsunpay-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-transactions-api-openapi.yml
- filename: orsunpay-com-usage-billing-api-openapi.yml
  format: yaml
  label: Orsun Pay Usage billing API
  slug: orsunpay-com-usage-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-usage-billing-api-openapi.yml
- filename: orsunpay-com-webhooks-api-openapi.yml
  format: yaml
  label: Orsun Pay Webhooks API
  slug: orsunpay-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orsunpay-com/openapi/orsunpay-com-webhooks-api-openapi.yml
auth_types: []
description: Authenticate server‑to‑server requests with your merchant API key in the x-api-key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Orsun Pay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orsun Pay declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Orsun Pay
provider_slug: orsunpay-com
scheme_count: 1
schemes:
- evidence: Authenticate server-to-server requests with your merchant API key in the x-api-key header.
  header: x-api-key
  how_to_obtain: Create or rotate a test or live API key in the merchant cabinet; the full key is shown once when created or rotated.
  location: header
  name: API Key
  type: apiKey
slug: orsunpay-com-authentication
source_filename: orsunpay-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.orsunpay.com/authentication.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.orsunpay.com/authentication.md\nsources:\n- https://docs.orsunpay.com/authentication.md\n- https://docs.orsunpay.com/quickstart.md\ndescription: Authenticate server‑to‑server requests with your merchant API key in the x-api-key header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Authenticate server-to-server requests with your merchant API key in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create or rotate a test or live API key in the merchant cabinet; the full key is shown once when created or rotated.\nnote: There is no OAuth flow or self‑service sign‑up endpoint.\ndocs: https://docs.orsunpay.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/orsunpay-com/authentication/orsunpay-com-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Payment Orchestration
- Checkout
- Payment Links
- Merchant Cabinet
- iGaming
- Crypto Payments
- Donations
---
