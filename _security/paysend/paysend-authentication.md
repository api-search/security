---
api_key_in:
- provisioned
auth_types:
- apiKey
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Paysend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paysend secures its APIs with apiKey and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paysend
provider_slug: paysend
scheme_count: 2
schemes:
- description: A partner-provisioned inbound API key issued by Paysend during enterprise onboarding. Not passed as a bearer token; it is a shared secret used both to identify the partner and as an input to the request signature.
  name: InboundAPIKey
  provisioning: enterprise onboarding (partner-provisioned)
  sources:
  - docs
  type: apiKey
- algorithms:
  - SHA-256
  - SHA-512
  description: HMAC-style request signature. For API calls the source string is the concatenation {RequestBody}{InboundAPIKey}; for status checks the source string is {globalId}{InboundAPIKey}. The agreed hash algorithm is applied to the source string and the resulting hash is hex-encoded into the header.
  encoding: hexadecimal
  header: X-OPP-Signature
  in: header
  name: X-OPP-Signature
  scheme: hmac-signature
  signature_string_api: '{RequestBody}{InboundAPIKey}'
  signature_string_status: '{globalId}{InboundAPIKey}'
  sources:
  - docs
  type: http
slug: paysend-authentication
source_filename: paysend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developer.paysend.com/authentication-and-idempotency/\ndocs: https://developer.paysend.com/authentication-and-idempotency/\nnote: >-\n  Derived from the Paysend Enterprise developer portal auth documentation rather\n  than an OpenAPI securitySchemes block (no downloadable spec is published). The\n  Payout API authenticates every request with an inbound API key plus an HMAC\n  digital signature carried in the X-OPP-Signature header. No OAuth2, OpenID\n  Connect, or mutual TLS is documented.\nsummary:\n  types: [apiKey, hmac-signature]\n  api_key_in: [provisioned]\n  oauth2_flows: []\nschemes:\n  - name: InboundAPIKey\n    type: apiKey\n    description: >-\n      A partner-provisioned inbound API key issued by Paysend during enterprise\n      onboarding. Not passed as a bearer token; it is a shared secret used both\n      to identify the partner and as an input to the request signature.\n    provisioning: enterprise onboarding\
  \ (partner-provisioned)\n    sources: [docs]\n  - name: X-OPP-Signature\n    type: http\n    scheme: hmac-signature\n    in: header\n    header: X-OPP-Signature\n    description: >-\n      HMAC-style request signature. For API calls the source string is the\n      concatenation {RequestBody}{InboundAPIKey}; for status checks the source\n      string is {globalId}{InboundAPIKey}. The agreed hash algorithm is applied\n      to the source string and the resulting hash is hex-encoded into the header.\n    algorithms: [SHA-256, SHA-512]\n    signature_string_api: '{RequestBody}{InboundAPIKey}'\n    signature_string_status: '{globalId}{InboundAPIKey}'\n    encoding: hexadecimal\n    sources: [docs]\nidempotency:\n  supported: true\n  mechanism: >-\n    Requests are made idempotent via two required header fields inside the JSON\n    request envelope: header.request.id (a unique idempotency key per request)\n    and header.request.date (the request timestamp, ISO 8601). The combination\n    of\
  \ the two guarantees an operation is not performed more than once.\n  fields:\n    - name: header.request.id\n      description: Unique idempotency key for each API request.\n    - name: header.request.date\n      description: Request timestamp (ISO 8601, e.g. 2024-08-15T14:30:00Z).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paysend/refs/heads/main/authentication/paysend-authentication.yml
summary_line: apiKey/hmac-signature · 2 schemes
tags:
- Payments
- United Kingdom
- Cross-Border
- Money Transfer
- Payouts
- Payment Processing
- FX
- Remittance
- Fintech
---
