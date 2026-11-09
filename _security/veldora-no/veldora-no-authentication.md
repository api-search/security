---
anonymous_access: false
api_key_in: []
api_specs:
- filename: veldora-no-addresses-api-openapi.yml
  format: yaml
  label: veldora-no Addresses API
  slug: veldora-no-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-addresses-api-openapi.yml
- filename: veldora-no-alerts-api-openapi.yml
  format: yaml
  label: veldora-no Alerts API
  slug: veldora-no-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-alerts-api-openapi.yml
- filename: veldora-no-companies-api-openapi.yml
  format: yaml
  label: veldora-no Companies API
  slug: veldora-no-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-companies-api-openapi.yml
- filename: veldora-no-exchange-rates-api-openapi.yml
  format: yaml
  label: veldora-no Exchange Rates API
  slug: veldora-no-exchange-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-exchange-rates-api-openapi.yml
- filename: veldora-no-fi-api-openapi.yml
  format: yaml
  label: veldora-no Fi API
  slug: veldora-no-fi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-fi-api-openapi.yml
- filename: veldora-no-health-api-openapi.yml
  format: yaml
  label: veldora-no Health API
  slug: veldora-no-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-health-api-openapi.yml
- filename: veldora-no-laws-api-openapi.yml
  format: yaml
  label: veldora-no Laws API
  slug: veldora-no-laws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-laws-api-openapi.yml
- filename: veldora-no-statistics-api-openapi.yml
  format: yaml
  label: veldora-no Statistics API
  slug: veldora-no-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-statistics-api-openapi.yml
- filename: veldora-no-tenders-api-openapi.yml
  format: yaml
  label: veldora-no Tenders API
  slug: veldora-no-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-tenders-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Veldora No Authentication
name_suffix: Authentication
oauth_flows: []
overview: veldora-no declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: veldora-no
provider_slug: veldora-no
scheme_count: 1
schemes:
- description: Authentication is performed via x402 payment on Base mainnet (eip155:8453) using USDC. No API keys or accounts.
  details:
    asset: USDC
    flow: Send request, receive 402 with PAYMENT-REQUIRED, sign EIP-3009 transferWithAuthorization, resend with PAYMENT-SIGNATURE.
    network: eip155:8453
  type: payment
slug: veldora-no-authentication
source_filename: veldora-no-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource:\n  - https://veldora.no/docs#authentication\nschemes:\n  - type: \"payment\"\n    description: \"Authentication is performed via x402 payment on Base mainnet (eip155:8453) using USDC. No API keys or accounts.\"\n    details:\n      network: \"eip155:8453\"\n      asset: \"USDC\"\n      flow: \"Send request, receive 402 with PAYMENT-REQUIRED, sign EIP-3009 transferWithAuthorization, resend with PAYMENT-SIGNATURE.\"\n"
source_yaml_url: https://artifacts.apis.io/veldora-no/authentication/veldora-no-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Norway
- Artificial Intelligence
- Public Data
---
