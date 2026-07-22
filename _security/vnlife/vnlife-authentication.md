---
api_key_in: []
auth_types:
- checksum-signature
- merchant-credential
description: ''
kind: authentication
layout: security
method: searched
name: Vnlife Authentication
name_suffix: Authentication
oauth_flows: []
overview: VNLIFE secures its APIs with checksum-signature and merchant-credential across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VNLIFE
provider_slug: vnlife
scheme_count: 2
schemes:
- description: Merchant/terminal identifier issued by VNPAY on onboarding.
  name: MerchantTerminal
  parameter: vnp_TmnCode
  type: credential
- algorithm: HMAC-SHA512
  applies_to:
  - Payment URL creation (vpcpay redirect)
  - Return URL verification
  - IPN callback verification
  - Merchant web API (transaction query / refund)
  canonicalization: Sort vnp_ parameters alphabetically by key, URL-encode values, concatenate key=value pairs with '&' (excluding vnp_SecureHash and vnp_SecureHashType), then HMAC-SHA512 with the merchant HashSecret.
  name: SecureHash
  parameter: vnp_SecureHash
  secret: vnp_HashSecret
  type: signature
slug: vnlife-authentication
source_filename: vnlife-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://sandbox.vnpayment.vn/apis/docs/thanh-toan-pay/pay.html\ndocs: https://sandbox.vnpayment.vn/apis/docs/huong-dan-tich-hop/\nsummary:\n  types: [checksum-signature, merchant-credential]\n  transport: query-string (redirect) + server-to-server IPN\n  scheme: HMAC-SHA512 message signature\nnote: >-\n  VNPAY has no OAuth/API-key bearer flow. Merchants are provisioned a Terminal\n  code (vnp_TmnCode) plus a secret hash key (vnp_HashSecret). Every request and\n  callback is signed with an HMAC-SHA512 checksum over the alphabetically-sorted,\n  URL-encoded vnp_ parameter set (excluding vnp_SecureHash), placed in\n  vnp_SecureHash. The receiver recomputes and compares to authenticate.\nschemes:\n- name: MerchantTerminal\n  type: credential\n  parameter: vnp_TmnCode\n  description: Merchant/terminal identifier issued by VNPAY on onboarding.\n- name: SecureHash\n  type: signature\n  algorithm: HMAC-SHA512\n  parameter: vnp_SecureHash\n\
  \  secret: vnp_HashSecret\n  canonicalization: >-\n    Sort vnp_ parameters alphabetically by key, URL-encode values, concatenate\n    key=value pairs with '&' (excluding vnp_SecureHash and vnp_SecureHashType),\n    then HMAC-SHA512 with the merchant HashSecret.\n  applies_to:\n  - Payment URL creation (vpcpay redirect)\n  - Return URL verification\n  - IPN callback verification\n  - Merchant web API (transaction query / refund)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vnlife/refs/heads/main/authentication/vnlife-authentication.yml
summary_line: checksum-signature/merchant-credential · 2 schemes
tags:
- Company
- Fintech
- Payments
- Payment Gateway
- QR Payments
- E-Commerce
- Vietnam
- Financial Services
---
