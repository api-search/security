---
api_key_in:
- header
api_specs:
- filename: openapi-payment-gateway.json
  format: json
  label: Cashfree Payment Gateway API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/openapi/openapi-payment-gateway.json
- filename: openapi-payouts.json
  format: json
  label: Cashfree Payouts API
  slug: payouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/openapi/openapi-payouts.json
- filename: openapi-verification.json
  format: json
  label: Cashfree Secure ID (Verification) API
  slug: secure-id
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/openapi/openapi-verification.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cashfree Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cashfree Payments secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cashfree Payments
provider_slug: cashfree
scheme_count: 6
schemes:
- description: Client app ID. You can find your app id in the [merchant dashboard](https://merchant.cashfree.com/merchants/pg/developers/api-keys?env=prod").
  in: header
  name: XClientID
  parameter: x-client-id
  sources:
  - openapi/openapi-payment-gateway.json
  - openapi/openapi-payouts.json
  - openapi/openapi-verification.json
  type: apiKey
- description: Client secret key. You can find your secret in the [merchant dashboard](https://merchant.cashfree.com/merchants/pg/developers/api-keys?env=prod").
  in: header
  name: XClientSecret
  parameter: x-client-secret
  sources:
  - openapi/openapi-payment-gateway.json
  - openapi/openapi-payouts.json
  - openapi/openapi-verification.json
  type: apiKey
- description: Use this if you do not want to pass the secret key and instead want to use the signature.
  in: header
  name: XClientSignatureHeader
  parameter: x-client-signature
  sources:
  - openapi/openapi-payment-gateway.json
  type: apiKey
- description: If you are partner and you are making an api call on behalf of a merchant
  in: header
  name: XPartnerAPIKey
  parameter: x-partner-apikey
  sources:
  - openapi/openapi-payment-gateway.json
  type: apiKey
- description: If you are partner use this to specify the merchant id if you don't have the merchant client app id
  in: header
  name: XPartnerMerchantID
  parameter: x-partner-merchantid
  sources:
  - openapi/openapi-payment-gateway.json
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi-verification.json
  type: http
slug: cashfree-authentication
source_filename: cashfree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-payment-gateway.json, openapi/openapi-payouts.json, openapi/openapi-verification.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: XClientID\n  type: apiKey\n  in: header\n  parameter: x-client-id\n  description: Client app ID. You can find your app id in the [merchant dashboard](https://merchant.cashfree.com/merchants/pg/developers/api-keys?env=prod\").\n  sources:\n  - openapi/openapi-payment-gateway.json\n  - openapi/openapi-payouts.json\n  - openapi/openapi-verification.json\n- name: XClientSecret\n  type: apiKey\n  in: header\n  parameter: x-client-secret\n  description: Client secret key. You can find your secret in the [merchant dashboard](https://merchant.cashfree.com/merchants/pg/developers/api-keys?env=prod\").\n  sources:\n  - openapi/openapi-payment-gateway.json\n  - openapi/openapi-payouts.json\n  - openapi/openapi-verification.json\n- name: XClientSignatureHeader\n\
  \  type: apiKey\n  in: header\n  parameter: x-client-signature\n  description: Use this if you do not want to pass the secret key and instead want to use the\n    signature.\n  sources:\n  - openapi/openapi-payment-gateway.json\n- name: XPartnerAPIKey\n  type: apiKey\n  in: header\n  parameter: x-partner-apikey\n  description: If you are partner and you are making an api call on behalf of a merchant\n  sources:\n  - openapi/openapi-payment-gateway.json\n- name: XPartnerMerchantID\n  type: apiKey\n  in: header\n  parameter: x-partner-merchantid\n  description: If you are partner use this to specify the merchant id if you don't have the\n    merchant client app id\n  sources:\n  - openapi/openapi-payment-gateway.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openapi-verification.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/authentication/cashfree-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Payments
- Payouts
- UPI
- India
- Payment Gateway
- Subscriptions
- Refunds
- QR Codes
- Net Banking
- Identity Verification
---
