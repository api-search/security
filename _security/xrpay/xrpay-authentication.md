---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xrpay-connected-account-api-openapi.yml
  format: yaml
  label: XRPay Connected account API
  slug: xrpay-connected-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-connected-account-api-openapi.yml
- filename: xrpay-payment-intents-api-openapi.yml
  format: yaml
  label: XRPay Payment intents API
  slug: xrpay-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-payment-intents-api-openapi.yml
- filename: xrpay-payouts-api-openapi.yml
  format: yaml
  label: XRPay Payouts API
  slug: xrpay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-payouts-api-openapi.yml
- filename: xrpay-payroll-api-openapi.yml
  format: yaml
  label: XRPay Payroll API
  slug: xrpay-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-payroll-api-openapi.yml
- filename: xrpay-refunds-api-openapi.yml
  format: yaml
  label: XRPay Refunds API
  slug: xrpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-refunds-api-openapi.yml
- filename: xrpay-sandbox-api-openapi.yml
  format: yaml
  label: XRPay Sandbox API
  slug: xrpay-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-sandbox-api-openapi.yml
- filename: xrpay-webhooks-api-openapi.yml
  format: yaml
  label: XRPay Webhooks API
  slug: xrpay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Xrpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: XRPay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: XRPay
provider_slug: xrpay
scheme_count: 1
schemes:
- description: Secret API key or XRPay Connect access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/xrpay-openapi.yml
  type: http
slug: xrpay-authentication
source_filename: xrpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/xrpay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Secret API key or XRPay Connect access token.\n  sources:\n  - openapi/xrpay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/authentication/xrpay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Merchant Payments
- Refunds
- Webhooks
- Fintech
---
