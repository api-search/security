---
api_key_in: []
api_specs:
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-checkout-api-openapi.yml
  format: yaml
  label: Klarna Checkout API
  slug: klarna-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-checkout-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-push-notifications-asyncapi.yml
  format: yaml
  label: Klarna Push Notifications
  slug: klarna-push-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/asyncapi/klarna-push-notifications-asyncapi.yml
- filename: klarna-captures-api-openapi.yml
  format: yaml
  label: Klarna Captures API
  slug: klarna-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-captures-api-openapi.yml
- filename: klarna-checkout-api-openapi.yml
  format: yaml
  label: Klarna Checkout API
  slug: klarna-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-checkout-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-hpp-api-openapi.yml
  format: yaml
  label: Klarna Hpp API
  slug: klarna-hpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-hpp-api-openapi.yml
- filename: klarna-merchant-urls-address-update-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.address Update API
  slug: klarna-merchant-urls-address-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-address-update-api-openapi.yml
- filename: klarna-merchant-urls-country-change-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.country Change API
  slug: klarna-merchant-urls-country-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-country-change-api-openapi.yml
- filename: klarna-merchant-urls-shipping-option-update-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.shipping Option Update API
  slug: klarna-merchant-urls-shipping-option-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-shipping-option-update-api-openapi.yml
- filename: klarna-merchant-urls-validation-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.validation API
  slug: klarna-merchant-urls-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-validation-api-openapi.yml
- filename: klarna-merchantcard-api-openapi.yml
  format: yaml
  label: Klarna Merchantcard API
  slug: klarna-merchantcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchantcard-api-openapi.yml
- filename: klarna-orders-api-openapi.yml
  format: yaml
  label: Klarna Orders API
  slug: klarna-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-orders-api-openapi.yml
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-payouts-api-openapi.yml
  format: yaml
  label: Klarna Payouts API
  slug: klarna-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payouts-api-openapi.yml
- filename: klarna-refunds-api-openapi.yml
  format: yaml
  label: Klarna Refunds API
  slug: klarna-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-refunds-api-openapi.yml
- filename: klarna-reports-api-openapi.yml
  format: yaml
  label: Klarna Reports API
  slug: klarna-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-reports-api-openapi.yml
- filename: klarna-transactions-api-openapi.yml
  format: yaml
  label: Klarna Transactions API
  slug: klarna-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Klarna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klarna secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klarna
provider_slug: klarna
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/klarna-settlements-api-openapi.yml
  - openapi/order-management-api-openapi.yml
  type: http
slug: klarna-authentication
source_filename: klarna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/klarna-settlements-api-openapi.yml, openapi/order-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/klarna-settlements-api-openapi.yml\n  - openapi/order-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/authentication/klarna-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- BNPL
- Payments
- Cards
- Shopping
---
