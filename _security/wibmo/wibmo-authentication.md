---
api_key_in: []
auth_types:
- payload-encryption
description: ''
kind: authentication
layout: security
method: searched
name: Wibmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: WIBMO secures its APIs with payload-encryption across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WIBMO
provider_slug: wibmo
scheme_count: 1
schemes:
- description: Per-operation Encrypt and Decrypt APIs wrap the request/response payloads; credentials are provisioned by Wibmo at onboarding. Evidenced by the Encrypt/Decrypt operation pairs across Prepaid customer onboarding, card management, and wallet management in the API reference.
  name: payloadEncryption
  scheme: encrypt-decrypt-envelope
  sources:
  - developer.wibmo.com/reference
  type: custom
slug: wibmo-authentication
source_filename: wibmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.wibmo.com/reference\ndocs: https://developer.wibmo.com/docs/getting-started\nnotes: >-\n  Wibmo publishes no machine-readable OpenAPI, so this profile is captured from the developer\n  reference. The Prepaid / Token Hub / Wallet APIs use a request-and-response payload encryption\n  model: each functional operation is paired with a dedicated \"Encrypt API\" (to encrypt the request\n  body) and \"Decrypt API\" (to decrypt the response), keyed on merchant/issuer credentials issued by\n  Wibmo during onboarding. This is an encryption-envelope scheme rather than OAuth2 or a simple\n  bearer key.\nsummary:\n  types: [payload-encryption]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: payloadEncryption\n    type: custom\n    scheme: encrypt-decrypt-envelope\n    description: >-\n      Per-operation Encrypt and Decrypt APIs wrap the request/response payloads; credentials are\n      provisioned by Wibmo\
  \ at onboarding. Evidenced by the Encrypt/Decrypt operation pairs across\n      Prepaid customer onboarding, card management, and wallet management in the API reference.\n    sources: [developer.wibmo.com/reference]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wibmo/refs/heads/main/authentication/wibmo-authentication.yml
summary_line: payload-encryption · 1 scheme
tags:
- Company
- Consumer
- Payments
- Fintech
- Payment Gateway
- Tokenization
- Fraud Detection
- 3-D Secure
- Authentication
- Digital Wallet
- Prepaid Cards
- India
---
