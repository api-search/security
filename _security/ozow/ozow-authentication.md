---
api_key_in: []
api_specs:
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Payments API
  slug: ozow-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Transactions API
  slug: ozow-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Bank List API
  slug: ozow-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Refunds API
  slug: ozow-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: modeled-from-docs
name: Ozow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ozow secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ozow
provider_slug: ozow
scheme_count: 2
schemes:
- headerName: ApiKey
  in: header
  name: ApiKey
  note: Merchant API key issued in the Ozow dashboard (dash.ozow.com), sent on payment and transaction-query requests alongside a SHA512 HashCheck field. The HashCheck is computed by concatenating the request fields in the documented order (SiteCode, CountryCode, CurrencyCode, Amount, TransactionReference, BankReference, CancelUrl, ErrorUrl, SuccessUrl, NotifyUrl, IsTest), appending the merchant PrivateKey, lower-casing the string, and taking the SHA512 hex digest. Incoming NotifyUrl notifications are verified the same way (concatenate response fields excluding Hash, append PrivateKey, lowercase, SHA512).
  sources:
  - openapi/ozow-openapi.yml
  - https://hub.ozow.com/docs
  - https://ozow.com/integrations
  type: apiKey
- bearerFormat: token
  name: BearerToken
  note: The Refunds and Payouts APIs authenticate with a reusable bearer token obtained from the Ozow identity/token service (a "Get Token" request), used until it expires, in addition to a per-request HashCheck.
  scheme: bearer
  sources:
  - https://hub.ozow.com/docs
  - https://api.i-pay.co.za/guide/refund
  type: http
slug: ozow-authentication
source_filename: ozow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: modeled-from-docs\nsource: openapi/ozow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  headerName: ApiKey\n  note: >-\n    Merchant API key issued in the Ozow dashboard (dash.ozow.com), sent on\n    payment and transaction-query requests alongside a SHA512 HashCheck field.\n    The HashCheck is computed by concatenating the request fields in the\n    documented order (SiteCode, CountryCode, CurrencyCode, Amount,\n    TransactionReference, BankReference, CancelUrl, ErrorUrl, SuccessUrl,\n    NotifyUrl, IsTest), appending the merchant PrivateKey, lower-casing the\n    string, and taking the SHA512 hex digest. Incoming NotifyUrl notifications\n    are verified the same way (concatenate response fields excluding Hash,\n    append PrivateKey, lowercase, SHA512).\n  sources:\n  - openapi/ozow-openapi.yml\n  - https://hub.ozow.com/docs\n  - https://ozow.com/integrations\n- name: BearerToken\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: token\n  note: >-\n    The Refunds and Payouts APIs authenticate with a reusable bearer token\n    obtained from the Ozow identity/token service (a \"Get Token\" request),\n    used until it expires, in addition to a per-request HashCheck.\n  sources:\n  - https://hub.ozow.com/docs\n  - https://api.i-pay.co.za/guide/refund\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/authentication/ozow-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Instant EFT
- Pay by Bank
- Fintech
- South Africa
---
