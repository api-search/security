---
api_key_in:
- header
api_specs:
- filename: neon-commerce-account-api-openapi.yml
  format: yaml
  label: Neon Commerce Account API
  slug: neon-commerce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-account-api-openapi.yml
- filename: neon-commerce-assets-api-openapi.yml
  format: yaml
  label: Neon Commerce Assets API
  slug: neon-commerce-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-assets-api-openapi.yml
- filename: neon-commerce-auth-api-openapi.yml
  format: yaml
  label: Neon Commerce Auth API
  slug: neon-commerce-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-auth-api-openapi.yml
- filename: neon-commerce-checkout-api-openapi.yml
  format: yaml
  label: Neon Commerce Checkout API
  slug: neon-commerce-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-checkout-api-openapi.yml
- filename: neon-commerce-client-api-openapi.yml
  format: yaml
  label: Neon Commerce Client API
  slug: neon-commerce-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-client-api-openapi.yml
- filename: neon-commerce-payouts-api-openapi.yml
  format: yaml
  label: Neon Commerce Payouts API
  slug: neon-commerce-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-payouts-api-openapi.yml
- filename: neon-commerce-prices-api-openapi.yml
  format: yaml
  label: Neon Commerce Prices API
  slug: neon-commerce-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-prices-api-openapi.yml
- filename: neon-commerce-pricing-sheet-api-openapi.yml
  format: yaml
  label: Neon Commerce Pricing Sheet API
  slug: neon-commerce-pricing-sheet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-pricing-sheet-api-openapi.yml
- filename: neon-commerce-purchases-api-openapi.yml
  format: yaml
  label: Neon Commerce Purchases API
  slug: neon-commerce-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-purchases-api-openapi.yml
- filename: neon-commerce-reports-api-openapi.yml
  format: yaml
  label: Neon Commerce Reports API
  slug: neon-commerce-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-reports-api-openapi.yml
- filename: neon-commerce-status-api-openapi.yml
  format: yaml
  label: Neon Commerce Status API
  slug: neon-commerce-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-status-api-openapi.yml
- filename: neon-commerce-storefront-api-openapi.yml
  format: yaml
  label: Neon Commerce Storefront API
  slug: neon-commerce-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-storefront-api-openapi.yml
- filename: neon-commerce-subscriptions-api-openapi.yml
  format: yaml
  label: Neon Commerce Subscriptions API
  slug: neon-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-subscriptions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Neon Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neon Commerce secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neon Commerce
provider_slug: neon-commerce
scheme_count: 3
schemes:
- description: 'Your Global API key, which spans across environments. Sandbox keys are prefixed with `gk_sandbox_`;

    production keys are prefixed with `gk_`. Find your keys in the Neon dashboard.'
  in: header
  name: GlobalApiKey
  parameter: X-Api-Key
  sources:
  - openapi/neon-commerce-account-openapi.yml
  - openapi/neon-commerce-assets-openapi.yml
  - openapi/neon-commerce-auth-openapi.yml
  - openapi/neon-commerce-checkout-openapi.yml
  - openapi/neon-commerce-payout-openapi.yml
  - openapi/neon-commerce-purchase-openapi.yml
  - openapi/neon-commerce-reports-openapi.yml
  - openapi/neon-commerce-storefront-openapi.yml
  - openapi/neon-commerce-subscriptions-openapi.yml
  type: apiKey
- description: 'Your Client key, used for client-side requests. Sandbox keys are prefixed with `ck_sandbox_`;

    production keys are prefixed with `ck_`. Find your keys in the Neon dashboard.'
  in: header
  name: ClientKey
  parameter: X-Client-Key
  sources:
  - openapi/neon-commerce-auth-openapi.yml
  - openapi/neon-commerce-storefront-openapi.yml
  type: apiKey
- description: 'A short-lived client token obtained from the `/client/token` endpoint, used for

    client-side requests to the Neon APIs.'
  in: header
  name: ClientToken
  parameter: X-Client-Token
  sources:
  - openapi/neon-commerce-checkout-openapi.yml
  - openapi/neon-commerce-purchase-openapi.yml
  type: apiKey
slug: neon-commerce-authentication
source_filename: neon-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/neon-commerce-account-openapi.yml, openapi/neon-commerce-assets-openapi.yml,\n  openapi/neon-commerce-auth-openapi.yml, openapi/neon-commerce-checkout-openapi.yml, openapi/neon-commerce-payout-openapi.yml,\n  openapi/neon-commerce-purchase-openapi.yml, openapi/neon-commerce-reports-openapi.yml, openapi/neon-commerce-storefront-openapi.yml,\n  openapi/neon-commerce-subscriptions-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: GlobalApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: |-\n    Your Global API key, which spans across environments. Sandbox keys are prefixed with `gk_sandbox_`;\n    production keys are prefixed with `gk_`. Find your keys in the Neon dashboard.\n  sources:\n  - openapi/neon-commerce-account-openapi.yml\n  - openapi/neon-commerce-assets-openapi.yml\n  - openapi/neon-commerce-auth-openapi.yml\n  - openapi/neon-commerce-checkout-openapi.yml\n\
  \  - openapi/neon-commerce-payout-openapi.yml\n  - openapi/neon-commerce-purchase-openapi.yml\n  - openapi/neon-commerce-reports-openapi.yml\n  - openapi/neon-commerce-storefront-openapi.yml\n  - openapi/neon-commerce-subscriptions-openapi.yml\n- name: ClientKey\n  type: apiKey\n  in: header\n  parameter: X-Client-Key\n  description: |-\n    Your Client key, used for client-side requests. Sandbox keys are prefixed with `ck_sandbox_`;\n    production keys are prefixed with `ck_`. Find your keys in the Neon dashboard.\n  sources:\n  - openapi/neon-commerce-auth-openapi.yml\n  - openapi/neon-commerce-storefront-openapi.yml\n- name: ClientToken\n  type: apiKey\n  in: header\n  parameter: X-Client-Token\n  description: |-\n    A short-lived client token obtained from the `/client/token` endpoint, used for\n    client-side requests to the Neon APIs.\n  sources:\n  - openapi/neon-commerce-checkout-openapi.yml\n  - openapi/neon-commerce-purchase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/authentication/neon-commerce-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Commerce
- Payments
- Gaming
- Checkout
- Storefront
- Direct-to-Consumer
- Subscriptions
- Merchant of Record
- Game Monetization
- Company
---
