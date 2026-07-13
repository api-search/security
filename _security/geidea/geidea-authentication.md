---
api_key_in: []
api_specs:
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Checkout API
  slug: geidea-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Direct API
  slug: geidea-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Tokenization API
  slug: geidea-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Transaction Management API
  slug: geidea-transaction-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
auth_types:
- http
- signature
description: ''
kind: authentication
layout: security
method: derived
name: Geidea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geidea secures its APIs with http and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Geidea
provider_slug: geidea
scheme_count: 2
schemes:
- description: HTTP Basic authentication. The merchant Public Key is the username and the API Password is the password, Base64-encoded into the standard Authorization header. Credentials are issued via the Geidea enablement team or the merchant portal under Payment Gateway -> Gateway Settings. The API Password is a secret and must never be exposed in a front-end; all Direct API calls must be made server-to-server.
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.geidea.net/docs/pre-requisites
  - openapi/geidea-openapi.yml
  type: http
- description: Requests additionally carry an HMAC request signature in the JSON body. The signature is an HMAC-SHA256 keyed by the API Password and Base64-encoded. For a Create Session request it is computed over a canonical concatenation of the merchant public key, amount, currency, merchant reference id, and timestamp; for merchant-initiated transactions it is computed over the merchant public key and session id. The exact canonical string per operation is documented in the Geidea API reference and should be confirmed before implementation.
  encoding: base64
  fieldName: signature
  in: body
  name: hmacSignature
  scheme: HMAC-SHA256
  sources:
  - https://docs.geidea.net/docs/merchant-initiated-mit
  - https://docs.geidea.net/reference/create-session-v2-1
  type: signature
slug: geidea-authentication
source_filename: geidea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: docs.geidea.net (Pre-requisites, API reference) + openapi/geidea-openapi.yml\nsummary:\n  types:\n  - http\n  - signature\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The merchant Public Key is the username and the API\n    Password is the password, Base64-encoded into the standard Authorization header.\n    Credentials are issued via the Geidea enablement team or the merchant portal\n    under Payment Gateway -> Gateway Settings. The API Password is a secret and must\n    never be exposed in a front-end; all Direct API calls must be made\n    server-to-server.\n  sources:\n  - https://docs.geidea.net/docs/pre-requisites\n  - openapi/geidea-openapi.yml\n- name: hmacSignature\n  type: signature\n  scheme: HMAC-SHA256\n  in: body\n  fieldName: signature\n  encoding: base64\n  description: >-\n    Requests additionally carry an HMAC request signature in the JSON\
  \ body. The\n    signature is an HMAC-SHA256 keyed by the API Password and Base64-encoded. For a\n    Create Session request it is computed over a canonical concatenation of the\n    merchant public key, amount, currency, merchant reference id, and timestamp; for\n    merchant-initiated transactions it is computed over the merchant public key and\n    session id. The exact canonical string per operation is documented in the Geidea\n    API reference and should be confirmed before implementation.\n  sources:\n  - https://docs.geidea.net/docs/merchant-initiated-mit\n  - https://docs.geidea.net/reference/create-session-v2-1\nnotes: >-\n  Two mechanisms are used together: HTTP Basic auth carries the merchant identity\n  and secret, and the per-request HMAC signature protects the integrity and\n  authenticity of the payload. Base hosts are region-specific:\n  api.ksamerchant.geidea.net (KSA), api.merchant.geidea.net (Egypt), and\n  api.geidea.ae (UAE).\nmaintainers:\n- FN: Kin Lane\n  email:\
  \ kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/authentication/geidea-authentication.yml
summary_line: http/signature · 2 schemes
tags:
- Payments
- Payment Gateway
- Saudi Arabia
- Egypt
- MENA
- mada
- Cards
- POS
- Checkout
- Fintech
---
