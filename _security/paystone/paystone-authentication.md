---
api_key_in: []
api_specs:
- filename: paystone-balance-portal-api-openapi.yml
  format: yaml
  label: Paystone Balance Portal API
  slug: paystone-balance-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-balance-portal-api-openapi.yml
- filename: paystone-client-management-api-openapi.yml
  format: yaml
  label: Paystone Client Management API
  slug: paystone-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-client-management-api-openapi.yml
- filename: paystone-contact-api-openapi.yml
  format: yaml
  label: Paystone Contact API
  slug: paystone-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-contact-api-openapi.yml
- filename: paystone-gift-account-type-api-openapi.yml
  format: yaml
  label: Paystone Gift Account Type API
  slug: paystone-gift-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-gift-account-type-api-openapi.yml
- filename: paystone-item-api-openapi.yml
  format: yaml
  label: Paystone Item API
  slug: paystone-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-item-api-openapi.yml
- filename: paystone-loyalty-account-type-api-openapi.yml
  format: yaml
  label: Paystone Loyalty Account Type API
  slug: paystone-loyalty-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-loyalty-account-type-api-openapi.yml
- filename: paystone-loyalty-transaction-api-openapi.yml
  format: yaml
  label: Paystone Loyalty Transaction API
  slug: paystone-loyalty-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-loyalty-transaction-api-openapi.yml
- filename: paystone-member-portal-api-openapi.yml
  format: yaml
  label: Paystone Member Portal API
  slug: paystone-member-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-member-portal-api-openapi.yml
- filename: paystone-merchant-management-api-openapi.yml
  format: yaml
  label: Paystone Merchant Management API
  slug: paystone-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-merchant-management-api-openapi.yml
- filename: paystone-prepaid-transaction-api-openapi.yml
  format: yaml
  label: Paystone Prepaid Transaction API
  slug: paystone-prepaid-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-prepaid-transaction-api-openapi.yml
- filename: paystone-promo-account-type-api-openapi.yml
  format: yaml
  label: Paystone Promo Account Type API
  slug: paystone-promo-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-promo-account-type-api-openapi.yml
- filename: paystone-reward-api-openapi.yml
  format: yaml
  label: Paystone Reward API
  slug: paystone-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-reward-api-openapi.yml
- filename: paystone-user-management-api-openapi.yml
  format: yaml
  label: Paystone User Management API
  slug: paystone-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-user-management-api-openapi.yml
- filename: paystone-webhook-management-api-openapi.yml
  format: yaml
  label: Paystone Webhook Management API
  slug: paystone-webhook-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-webhook-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paystone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paystone secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paystone
provider_slug: paystone
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter your JWT token (without the "Bearer" prefix).
  name: JWT
  scheme: bearer
  sources:
  - openapi/paystone-datacandy-openapi.yml
  type: http
slug: paystone-authentication
source_filename: paystone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/paystone-datacandy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter your JWT token (without the \"Bearer\" prefix).\n  sources:\n  - openapi/paystone-datacandy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/authentication/paystone-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Canada
- Payment Processing
- Acquiring
- Gift Cards
- Loyalty
- Subscription
- Billing
- Merchant Services
---
