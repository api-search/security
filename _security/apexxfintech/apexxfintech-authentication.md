---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apexxfintech-alternative-payment-methods-api-openapi.yml
  format: yaml
  label: Apexxfintech Alternative Payment Methods API
  slug: apexxfintech-alternative-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-alternative-payment-methods-api-openapi.yml
- filename: apexxfintech-buy-now-pay-later-api-openapi.yml
  format: yaml
  label: Apexxfintech Buy Now Pay Later API
  slug: apexxfintech-buy-now-pay-later-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-buy-now-pay-later-api-openapi.yml
- filename: apexxfintech-create-and-manage-card-token-api-openapi.yml
  format: yaml
  label: Apexxfintech Create And Manage Card Token API
  slug: apexxfintech-create-and-manage-card-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-create-and-manage-card-token-api-openapi.yml
- filename: apexxfintech-credit-transaction-api-openapi.yml
  format: yaml
  label: Apexxfintech Credit Transaction API
  slug: apexxfintech-credit-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-credit-transaction-api-openapi.yml
- filename: apexxfintech-get-transactions-api-openapi.yml
  format: yaml
  label: Apexxfintech Get Transactions API
  slug: apexxfintech-get-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-get-transactions-api-openapi.yml
- filename: apexxfintech-hosted-token-api-openapi.yml
  format: yaml
  label: Apexxfintech Hosted Token API
  slug: apexxfintech-hosted-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-hosted-token-api-openapi.yml
- filename: apexxfintech-sdk-api-openapi.yml
  format: yaml
  label: Apexxfintech SDK API
  slug: apexxfintech-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-sdk-api-openapi.yml
- filename: apexxfintech-server-side-encryption-api-openapi.yml
  format: yaml
  label: Apexxfintech SERVER-SIDE ENCRYPTION API
  slug: apexxfintech-server-side-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-server-side-encryption-api-openapi.yml
- filename: apexxfintech-standalone-services-api-openapi.yml
  format: yaml
  label: Apexxfintech STANDALONE SERVICES API
  slug: apexxfintech-standalone-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-standalone-services-api-openapi.yml
- filename: apexxfintech-transaction-hosted-payment-api-openapi.yml
  format: yaml
  label: Apexxfintech Transaction Hosted Payment API
  slug: apexxfintech-transaction-hosted-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-transaction-hosted-payment-api-openapi.yml
- filename: apexxfintech-transaction-payment-api-openapi.yml
  format: yaml
  label: Apexxfintech Transaction Payment API
  slug: apexxfintech-transaction-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-transaction-payment-api-openapi.yml
- filename: apexxfintech-transaction-update-api-openapi.yml
  format: yaml
  label: Apexxfintech Transaction Update API
  slug: apexxfintech-transaction-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-transaction-update-api-openapi.yml
auth_types: []
description: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called X-APIKEY. The value of this header must be the API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apexxfintech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apexxfintech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apexxfintech
provider_slug: apexxfintech
scheme_count: 1
schemes:
- evidence: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called X-APIKEY. The value of this header must be the API key.
  header: X-APIKEY
  location: header
  name: X-APIKEY
  type: apiKey
slug: apexxfintech-authentication
source_filename: apexxfintech-authentication.yml
source_heading: Authentication Profile
source_url: https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST\nsources:\n- https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST\n- https://sandbox.apexx.global/atomic/redoc/api/doc\ndescription: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called\n  X-APIKEY. The value of this header must be the API key.\nschemes:\n- type: apiKey\n  name: X-APIKEY\n  evidence: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called\n    X-APIKEY. The value of this header must be the API key.\n  location: header\n  header: X-APIKEY\ndocs: https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/authentication/apexxfintech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Fintech
- Orchestration
- Global
---
