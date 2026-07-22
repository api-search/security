---
api_key_in: []
api_specs:
- filename: paypay-opa-openapi-original.json
  format: json
  label: PayPay Open Payment API (OPA v2)
  slug: paypay-open-payment-api-opa-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypay/refs/heads/main/openapi/paypay-opa-openapi-original.json
auth_types:
- http
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Paypay Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayPay secures its APIs with http and hmac across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayPay
provider_slug: paypay
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: Basic
  sources:
  - openapi/paypay-opa-openapi-original.json
  type: http
- algorithm: HMAC-SHA256
  documented: true
  format: hmac OPA:{ApiKey}:{macData}:{nonce}:{epoch}:{hash}
  header: Authorization
  name: HmacOPA
  parameters:
    api_key: API key generated in the Developer/Merchant Panel
    api_secret: API key secret generated in the Developer/Merchant Panel
    epoch: epoch seconds, validated server-side to be within 2 minutes
    hash: base64 HMAC over method + URI + content-type + epoch + nonce + body hash
    nonce: random string (recommended length 8)
  scheme: hmac
  source: https://www.paypay.ne.jp/opa/doc/v1.0/api_authorization.html
  type: http
slug: paypay-authentication
source_filename: paypay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/paypay-opa-openapi-original.json\ndocs: https://www.paypay.ne.jp/opa/doc/v1.0/api_authorization.html\nsummary:\n  types:\n  - http\n  - hmac\n  note: >-\n    The OpenAPI declares a simplified BasicAuth (http Basic) security scheme, but\n    the PayPay Open Payment API (OPA) is actually secured with a custom HMAC-SHA256\n    request signature. Merchants obtain an API key + API secret from the PayPay\n    Developer / Merchant Panel (separate keys per environment).\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: Basic\n  sources:\n  - openapi/paypay-opa-openapi-original.json\n- name: HmacOPA\n  type: http\n  scheme: hmac\n  documented: true\n  header: Authorization\n  format: 'hmac OPA:{ApiKey}:{macData}:{nonce}:{epoch}:{hash}'\n  algorithm: HMAC-SHA256\n  parameters:\n    api_key: API key generated in the Developer/Merchant Panel\n    api_secret: API key secret generated in the Developer/Merchant Panel\n    nonce:\
  \ random string (recommended length 8)\n    epoch: epoch seconds, validated server-side to be within 2 minutes\n    hash: base64 HMAC over method + URI + content-type + epoch + nonce + body hash\n  source: https://www.paypay.ne.jp/opa/doc/v1.0/api_authorization.html\nmerchant_scoping:\n  note: >-\n    Every request must also carry the merchant identifier, via the\n    X-ASSUME-MERCHANT HTTP header or the ?assumeMerchant={MerchantId} query\n    parameter (query takes precedence when both are supplied).\n  header: X-ASSUME-MERCHANT\n  query: assumeMerchant\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypay/refs/heads/main/authentication/paypay-authentication.yml
summary_line: http/hmac · 2 schemes
tags:
- Company
- Fintech
- Payments
- Mobile Payments
- QR Code Payments
- Digital Wallet
- Japan
- Merchant Payments
---
