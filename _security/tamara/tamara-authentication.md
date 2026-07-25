---
api_key_in: []
api_specs:
- filename: tamara-orders-api-openapi.yml
  format: yaml
  label: Tamara Orders API
  slug: tamara-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-orders-api-openapi.yml
- filename: tamara-in-store-checkout-api-openapi.yml
  format: yaml
  label: Tamara In-Store Checkout API
  slug: tamara-in-store-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-in-store-checkout-api-openapi.yml
- filename: tamara-webhooks-api-openapi.yml
  format: yaml
  label: Tamara Webhooks API
  slug: tamara-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-webhooks-api-openapi.yml
- filename: tamara-disputes-api-openapi.yml
  format: yaml
  label: Tamara Disputes API
  slug: tamara-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-disputes-api-openapi.yml
- filename: tamara-eligibility-api-openapi.yml
  format: yaml
  label: Tamara Pre-Checkout Eligibility API
  slug: tamara-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-eligibility-api-openapi.yml
- filename: tamara-captures-api-openapi.yml
  format: yaml
  label: Tamara Captures API
  slug: tamara-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-captures-api-openapi.yml
- filename: tamara-channel-partner-webhooks-api-openapi.yml
  format: yaml
  label: Tamara Channel Partner Webhooks API
  slug: tamara-channel-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-channel-partner-webhooks-api-openapi.yml
- filename: tamara-checkout-sessions-api-openapi.yml
  format: yaml
  label: Tamara Checkout Sessions API
  slug: tamara-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-checkout-sessions-api-openapi.yml
- filename: tamara-merchant-api-keys-api-openapi.yml
  format: yaml
  label: Tamara Merchant API Keys API
  slug: tamara-merchant-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-merchant-api-keys-api-openapi.yml
- filename: tamara-merchant-onboarding-api-openapi.yml
  format: yaml
  label: Tamara Merchant Onboarding API
  slug: tamara-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-merchant-onboarding-api-openapi.yml
- filename: tamara-refunds-api-openapi.yml
  format: yaml
  label: Tamara Refunds API
  slug: tamara-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-refunds-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tamara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tamara secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tamara
provider_slug: tamara
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tamara-channel-partners-api-openapi.yml
  - openapi/tamara-checkout-api-openapi.yml
  - openapi/tamara-disputes-api-openapi.yml
  - openapi/tamara-eligibility-api-openapi.yml
  - openapi/tamara-in-store-checkout-api-openapi.yml
  - openapi/tamara-orders-api-openapi.yml
  - openapi/tamara-payments-api-openapi.yml
  - openapi/tamara-webhooks-api-openapi.yml
  type: http
slug: tamara-authentication
source_filename: tamara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tamara-channel-partners-api-openapi.yml, openapi/tamara-checkout-api-openapi.yml,\n  openapi/tamara-disputes-api-openapi.yml, openapi/tamara-eligibility-api-openapi.yml, openapi/tamara-in-store-checkout-api-openapi.yml,\n  openapi/tamara-orders-api-openapi.yml, openapi/tamara-payments-api-openapi.yml, openapi/tamara-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tamara-channel-partners-api-openapi.yml\n  - openapi/tamara-checkout-api-openapi.yml\n  - openapi/tamara-disputes-api-openapi.yml\n  - openapi/tamara-eligibility-api-openapi.yml\n  - openapi/tamara-in-store-checkout-api-openapi.yml\n  - openapi/tamara-orders-api-openapi.yml\n  - openapi/tamara-payments-api-openapi.yml\n  - openapi/tamara-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/authentication/tamara-authentication.yml
summary_line: http · 1 scheme
tags:
- BNPL
- Buy Now Pay Later
- Fintech
- Payments
- Checkout
- Shariah Compliant
- MENA
- Saudi Arabia
- UAE
- Installments
- Pay Later
- Merchant Services
- Orders
- Refunds
- Captures
- Webhooks
- Disputes
- Channel Partners
- E-commerce
- POS
---
