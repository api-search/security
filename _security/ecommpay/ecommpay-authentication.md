---
api_key_in:
- request-body-parameter
auth_types:
- signature-hmac
description: ''
kind: authentication
layout: security
method: searched
name: Ecommpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: ECOMMPAY secures its APIs with signature-hmac across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ECOMMPAY
provider_slug: ecommpay
scheme_count: 1
schemes:
- algorithm: HMAC-SHA-512
  applies_to:
  - outgoing merchant requests (e.g. checkout, refund, payout)
  - inbound callbacks (verify signature before trusting)
  - certain synchronous responses (verify signature)
  encoding: base64
  identifier_parameter: project_id
  key: per-project secret key
  name: ProjectSignature
  procedure: Build the message from all request parameters except the signature; compute the HMAC-SHA-512 over it with the project secret key; Base64-encode the result and send it in the signature parameter. To verify a callback, remove the signature parameter, recompute the HMAC over the remaining body, and compare - matching signatures confirm authenticity and integrity.
  sdk_support: Signature generation/verification is implemented by the official Payment Page SDKs (PHP, JS, Python, Java, Go, .NET, iOS, Android) - see packages/.
  signature_parameter: signature
  transport: HTTPS (TLS 1.2+)
  type: custom-signature
slug: ecommpay-authentication
source_filename: ecommpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://developers.ecommpay.com/en/en_Gate_Integration_About.html\ndocs:\n  gate_signature: https://developers.ecommpay.com/en/en_gate_signature_intro.html\n  data_signature: https://developers.ecommpay.com/en/en_dbl_signature_intro.html\n  callbacks: https://developers.ecommpay.com/en/en_platform_callbacks.html\nnote: >-\n  ECOMMPAY does not use OAuth2 or bearer tokens. Every request is identified by a\n  numeric project_id (issued to the merchant) and authenticated with a per-request\n  HMAC digital signature computed over the request parameters using the project's\n  secret key. The same signature scheme is applied in reverse to verify inbound\n  callbacks. There are no OAuth scopes; there is no OpenAPI securityScheme to derive\n  from because ECOMMPAY publishes no downloadable OpenAPI (its references are\n  Stoplight Elements SPAs). This profile is therefore searched from the docs, not\n  derived from a spec.\nsummary:\n\
  \  types: [signature-hmac]\n  token_based: false\n  oauth2: false\n  api_key_in: [request-body-parameter]\nschemes:\n  - name: ProjectSignature\n    type: custom-signature\n    algorithm: HMAC-SHA-512\n    encoding: base64\n    key: per-project secret key\n    identifier_parameter: project_id\n    signature_parameter: signature\n    applies_to:\n      - outgoing merchant requests (e.g. checkout, refund, payout)\n      - inbound callbacks (verify signature before trusting)\n      - certain synchronous responses (verify signature)\n    procedure: >-\n      Build the message from all request parameters except the signature; compute the\n      HMAC-SHA-512 over it with the project secret key; Base64-encode the result and\n      send it in the signature parameter. To verify a callback, remove the signature\n      parameter, recompute the HMAC over the remaining body, and compare - matching\n      signatures confirm authenticity and integrity.\n    transport: HTTPS (TLS 1.2+)\n    sdk_support:\
  \ >-\n      Signature generation/verification is implemented by the official Payment Page\n      SDKs (PHP, JS, Python, Java, Go, .NET, iOS, Android) - see packages/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecommpay/refs/heads/main/authentication/ecommpay-authentication.yml
summary_line: signature-hmac · 1 scheme
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- Alternative Payment Methods
- Open Banking
- Payouts
- Cross-Border
- Fraud
---
