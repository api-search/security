---
api_key_in:
- header
api_specs:
- filename: rye-betas-api-openapi.yml
  format: yaml
  label: Rye Betas API
  slug: rye-betas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-betas-api-openapi.yml
- filename: rye-billing-api-openapi.yml
  format: yaml
  label: Rye Billing API
  slug: rye-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-billing-api-openapi.yml
- filename: rye-brands-api-openapi.yml
  format: yaml
  label: Rye Brands API
  slug: rye-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-brands-api-openapi.yml
- filename: rye-checkout-intents-api-openapi.yml
  format: yaml
  label: Rye Checkout Intents API
  slug: rye-checkout-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-checkout-intents-api-openapi.yml
- filename: rye-commissions-api-openapi.yml
  format: yaml
  label: Rye Commissions API
  slug: rye-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-commissions-api-openapi.yml
- filename: rye-events-api-openapi.yml
  format: yaml
  label: Rye Events API
  slug: rye-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-events-api-openapi.yml
- filename: rye-merchant-connectors-api-openapi.yml
  format: yaml
  label: Rye Merchant Connectors API
  slug: rye-merchant-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-merchant-connectors-api-openapi.yml
- filename: rye-orders-api-openapi.yml
  format: yaml
  label: Rye Orders API
  slug: rye-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-orders-api-openapi.yml
- filename: rye-payment-gateways-api-openapi.yml
  format: yaml
  label: Rye Payment Gateways API
  slug: rye-payment-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-payment-gateways-api-openapi.yml
- filename: rye-products-api-openapi.yml
  format: yaml
  label: Rye Products API
  slug: rye-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-products-api-openapi.yml
- filename: rye-returns-api-openapi.yml
  format: yaml
  label: Rye Returns API
  slug: rye-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-returns-api-openapi.yml
- filename: rye-shipments-api-openapi.yml
  format: yaml
  label: Rye Shipments API
  slug: rye-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-shipments-api-openapi.yml
- filename: rye-test-helpers-api-openapi.yml
  format: yaml
  label: Rye Test Helpers API
  slug: rye-test-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-test-helpers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rye secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rye
provider_slug: rye
scheme_count: 1
schemes:
- description: Rye API key
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/rye-checkout-intents-openapi-original.yml
  type: apiKey
slug: rye-authentication
source_filename: rye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/rye-checkout-intents-openapi-original.yml\ndocs: https://rye.com/docs/api-v2/authorization\nnotes: >-\n  API-key auth via the Authorization header. Docs show \"Basic $RYE_API_KEY\" and\n  \"Bearer YOUR_API_KEY\" forms; keys are per-environment (staging vs production keys\n  are not interchangeable). No OAuth2/OIDC - no scope surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Rye API key\n  sources:\n  - openapi/rye-checkout-intents-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/authentication/rye-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Commerce
- E-Commerce
- Checkout
- Payments
- Agentic Commerce
- AI Agents
- Universal Checkout
- Shopping
---
