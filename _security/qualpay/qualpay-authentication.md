---
anonymous_access: false
api_key_in: []
api_specs:
- filename: qualpay-account-updater-api-openapi.yml
  format: yaml
  label: Qualpay Account Updater API
  slug: qualpay-account-updater-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-account-updater-api-openapi.yml
- filename: qualpay-application-boarding-api-openapi.yml
  format: yaml
  label: Qualpay Application Boarding API
  slug: qualpay-application-boarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-application-boarding-api-openapi.yml
- filename: qualpay-checkout-api-openapi.yml
  format: yaml
  label: Qualpay Checkout API
  slug: qualpay-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-checkout-api-openapi.yml
- filename: qualpay-customer-vault-api-openapi.yml
  format: yaml
  label: Qualpay Customer Vault API
  slug: qualpay-customer-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-customer-vault-api-openapi.yml
- filename: qualpay-disputes-v0-5-api-openapi.yml
  format: yaml
  label: Qualpay Disputes v0.5 API
  slug: qualpay-disputes-v0-5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-disputes-v0-5-api-openapi.yml
- filename: qualpay-disputes-v1-0-api-openapi.yml
  format: yaml
  label: Qualpay Disputes v1.0 API
  slug: qualpay-disputes-v1-0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-disputes-v1-0-api-openapi.yml
- filename: qualpay-embedded-fields-api-openapi.yml
  format: yaml
  label: Qualpay Embedded Fields API
  slug: qualpay-embedded-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-embedded-fields-api-openapi.yml
- filename: qualpay-integrator-api-openapi.yml
  format: yaml
  label: Qualpay Integrator API
  slug: qualpay-integrator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-integrator-api-openapi.yml
- filename: qualpay-invoicing-api-openapi.yml
  format: yaml
  label: Qualpay Invoicing API
  slug: qualpay-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-invoicing-api-openapi.yml
- filename: qualpay-payee-vault-api-openapi.yml
  format: yaml
  label: Qualpay Payee Vault API
  slug: qualpay-payee-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-payee-vault-api-openapi.yml
- filename: qualpay-payment-gateway-api-openapi.yml
  format: yaml
  label: Qualpay Payment Gateway API
  slug: qualpay-payment-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-payment-gateway-api-openapi.yml
- filename: qualpay-recurring-billing-api-openapi.yml
  format: yaml
  label: Qualpay Recurring Billing API
  slug: qualpay-recurring-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-recurring-billing-api-openapi.yml
- filename: qualpay-reporting-api-openapi.yml
  format: yaml
  label: Qualpay Reporting API
  slug: qualpay-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-reporting-api-openapi.yml
- filename: qualpay-token-api-openapi.yml
  format: yaml
  label: Qualpay Token API
  slug: qualpay-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-token-api-openapi.yml
- filename: qualpay-transaction-api-openapi.yml
  format: yaml
  label: Qualpay Transaction API
  slug: qualpay-transaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-transaction-api-openapi.yml
- filename: qualpay-webhooks-api-openapi.yml
  format: yaml
  label: Qualpay Webhooks API
  slug: qualpay-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Qualpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qualpay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qualpay
provider_slug: qualpay
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/qualpay-apis-api-openapi.yml
  type: http
slug: qualpay-authentication
source_filename: qualpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: derived\nsource: openapi/qualpay-apis-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/qualpay-apis-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/qualpay/authentication/qualpay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Processing
- Merchant Services
- B2B Payments
- Reporting
- Tokenization
---
