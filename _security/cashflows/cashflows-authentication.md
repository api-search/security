---
api_key_in:
- header
auth_types:
- apiKey
- http-hash-signature
- credential-pair
description: ''
kind: authentication
layout: security
method: searched
name: Cashflows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cashflows secures its APIs with apiKey, http-hash-signature, and credential-pair across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cashflows
provider_slug: cashflows
scheme_count: 3
schemes:
- api: cashflows-gateway-api
  in: header
  name: GatewaySignedRequest
  parameters:
  - description: Unique merchant account / configuration identifier.
    name: ConfigurationId
  - description: SHA2-512 hash of the request message body concatenated with the account API key, encoded as a hex string. Signs every request so the gateway can verify message integrity and origin. Repeated signature failures lock the account.
    name: Hash
  sources:
  - docs
  type: apiKey
- api: cashflows-remote-authentication-api
  in: body
  name: RemoteAuthCredentials
  parameters:
  - description: Profile / Merchant ID.
    name: auth_id
  - description: Authentication password for the acquiring-network connection.
    name: auth_pass
  - description: Additional hash required for credit (payout) transactions.
    name: security_hash
  sources:
  - docs
  type: credential-pair
- api: cashflows-payments-api
  in: header
  name: PaymentsSignedRequest
  parameters:
  - description: Merchant identifier included on every request.
    name: MerchantId
  - description: SHA2-512 signature over the request body, as with the Gateway.
    name: Hash
  sources:
  - docs
  type: http-hash-signature
slug: cashflows-authentication
source_filename: cashflows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developer.cashflows.com/api_reference/api_reference_overview.html\ndocs: https://developer.cashflows.com/getting_started/getting_started.html\nsummary:\n  types: [apiKey, http-hash-signature, credential-pair]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Cashflows uses header-based credentials and request signing, not OAuth.\n    Each API family authenticates differently. No OpenAPI securitySchemes are\n    published; this profile is derived from the hand-authored API reference.\nschemes:\n  - name: GatewaySignedRequest\n    api: cashflows-gateway-api\n    type: apiKey\n    in: header\n    parameters:\n      - name: ConfigurationId\n        description: Unique merchant account / configuration identifier.\n      - name: Hash\n        description: >-\n          SHA2-512 hash of the request message body concatenated with the\n          account API key, encoded as a hex string. Signs every request so the\n\
  \          gateway can verify message integrity and origin. Repeated signature\n          failures lock the account.\n    sources: [docs]\n  - name: RemoteAuthCredentials\n    api: cashflows-remote-authentication-api\n    type: credential-pair\n    in: body\n    parameters:\n      - name: auth_id\n        description: Profile / Merchant ID.\n      - name: auth_pass\n        description: Authentication password for the acquiring-network connection.\n      - name: security_hash\n        description: Additional hash required for credit (payout) transactions.\n    sources: [docs]\n  - name: PaymentsSignedRequest\n    api: cashflows-payments-api\n    type: http-hash-signature\n    in: header\n    parameters:\n      - name: MerchantId\n        description: Merchant identifier included on every request.\n      - name: Hash\n        description: SHA2-512 signature over the request body, as with the Gateway.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashflows/refs/heads/main/authentication/cashflows-authentication.yml
summary_line: apiKey/http-hash-signature/credential-pair · 3 schemes
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- In-Person Payments
- 3-D Secure
- Recurring Payments
- Webhooks
---
