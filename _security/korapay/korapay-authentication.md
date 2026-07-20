---
api_key_in: []
api_specs:
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Charges API
  slug: korapay-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Payouts API
  slug: korapay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Virtual Bank Accounts API
  slug: korapay-virtual-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Balances API
  slug: korapay-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Refunds API
  slug: korapay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Currency Conversion API
  slug: korapay-currency-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Misc Utilities API
  slug: korapay-misc-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
auth_types:
- http
- hmac
- encryption
description: ''
kind: authentication
layout: security
method: documented
name: Korapay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kora secures its APIs with http, hmac, and encryption across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kora
provider_slug: korapay
scheme_count: 4
schemes:
- description: 'Secret API key (sk_...) passed as `Authorization: Bearer [example key]`. Required for server-side and financial operations - payouts, balances, virtual bank accounts, refunds, conversions, and charge verification. Keep confidential; never expose in client-side code. Test and Live modes use different secret keys.'
  name: secretKeyAuth
  scheme: bearer
  sources:
  - https://developers.korapay.com/docs/api-keys
  - https://developers.korapay.com/docs/balance-api
  type: http
- description: Public API key (pk_...) used from client-side code to initiate transactions (for example, initializing a checkout charge). Non-sensitive; cannot access financial data or modify the account beyond initiating transactions. Test and Live modes use different public keys.
  name: publicKeyAuth
  scheme: bearer
  sources:
  - https://developers.korapay.com/docs/api-keys
  type: http
- description: Card charge payloads must be AES-256 encrypted with your account encryption key and submitted as a single `charge_data` string to POST /charges/card. Card payments additionally require the feature to be enabled on your account and PCI DSS Level 1 certification.
  name: cardPayloadEncryption
  scheme: AES-256
  sources:
  - https://developers.korapay.com/docs/accepting-card-payments-with-apis
  type: encryption
- description: Webhook requests from Kora carry an `x-korapay-signature` header that is an HMAC SHA-256 of ONLY the `data` object of the payload, signed with your secret key. Recompute and compare before delivering value to guarantee the request originated from Kora.
  header: x-korapay-signature
  name: webhookSignature
  scheme: HMAC-SHA256
  sources:
  - https://developers.korapay.com/docs/webhooks
  type: hmac
slug: korapay-authentication
source_filename: korapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://developers.korapay.com/docs/api-keys\nsummary:\n  types:\n  - http\n  - hmac\n  - encryption\nschemes:\n- name: secretKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Secret API key (sk_...) passed as `Authorization: Bearer [example key]`.\n    Required for server-side and financial operations - payouts, balances, virtual\n    bank accounts, refunds, conversions, and charge verification. Keep confidential;\n    never expose in client-side code. Test and Live modes use different secret keys.'\n  sources:\n  - https://developers.korapay.com/docs/api-keys\n  - https://developers.korapay.com/docs/balance-api\n- name: publicKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Public API key (pk_...) used from client-side code to initiate\n    transactions (for example, initializing a checkout charge). Non-sensitive; cannot\n    access financial data or modify the account beyond initiating transactions. Test\n\
  \    and Live modes use different public keys.'\n  sources:\n  - https://developers.korapay.com/docs/api-keys\n- name: cardPayloadEncryption\n  type: encryption\n  scheme: AES-256\n  description: 'Card charge payloads must be AES-256 encrypted with your account\n    encryption key and submitted as a single `charge_data` string to POST /charges/card.\n    Card payments additionally require the feature to be enabled on your account and\n    PCI DSS Level 1 certification.'\n  sources:\n  - https://developers.korapay.com/docs/accepting-card-payments-with-apis\n- name: webhookSignature\n  type: hmac\n  scheme: HMAC-SHA256\n  header: x-korapay-signature\n  description: 'Webhook requests from Kora carry an `x-korapay-signature` header that\n    is an HMAC SHA-256 of ONLY the `data` object of the payload, signed with your\n    secret key. Recompute and compare before delivering value to guarantee the\n    request originated from Kora.'\n  sources:\n  - https://developers.korapay.com/docs/webhooks\n\
  notes: >-\n  Kora uses API-key authentication (no OAuth). Every account has separate Test and\n  Live keys; ensure you use the correct mode's keys. Payout IP whitelisting is also\n  available on the dashboard as an additional control.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/authentication/korapay-authentication.yml
summary_line: http/hmac/encryption · 4 schemes
tags:
- Payments
- Payment Gateway
- Africa
- Nigeria
- Collections
- Payouts
- Disbursements
- Virtual Bank Account
- Cards
- Fintech
---
