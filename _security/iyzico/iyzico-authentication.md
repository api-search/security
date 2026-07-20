---
api_key_in: []
auth_types:
- custom-hmac
description: ''
kind: authentication
layout: security
method: searched
name: Iyzico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iyzico secures its APIs with custom-hmac across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Iyzico
provider_slug: iyzico
scheme_count: 1
schemes:
- additional_headers:
  - description: Randomly generated per-call value; historically the SHA1 random key.
    name: x-iyzi-rnd
  algorithm: HMACSHA256
  components:
    apiKey: Unique API key assigned to the merchant account (sandbox keys are prefixed "sandbox-").
    randomKey: Per-request nonce (formerly the x-iyzi-rnd random key).
    secretKey: Secret key paired with the apiKey; never transmitted, used to sign.
  description: iyzico authentication aligns with Basic Auth principles but signs each request. The signature is HMACSHA256(randomKey + uri.path + request.body, secretKey); the authorization string "apiKey:<apiKey>&randomKey:<randomKey>&signature:<encryptedData>" is Base64 encoded and sent as "IYZWSv2 <base64EncodedAuthorization>" in the Authorization header.
  format: IYZWSv2 <base64EncodedAuthorization>
  header: Authorization
  in: header
  legacy:
  - name: IYZWS (v1)
    note: Earlier SHA1-based authorization scheme, superseded by IYZWSv2 (HMACSHA256).
    status: deprecated
  name: IYZWSv2
  type: apiKey-hmac
slug: iyzico-authentication
source_filename: iyzico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.iyzico.com/en/getting-started/preliminaries/authentication/hmacsha256-auth\ndocs: https://docs.iyzico.com/en/getting-started/preliminaries/authentication\nsummary:\n  types: [custom-hmac]\n  scheme: IYZWSv2\n  credentials: [apiKey, secretKey]\n  transport: header\n  note: >-\n    No OpenAPI securitySchemes captured (no machine-readable spec harvested); the\n    profile below is transcribed from the published HMACSHA256 authentication docs.\nschemes:\n- name: IYZWSv2\n  type: apiKey-hmac\n  in: header\n  header: Authorization\n  format: 'IYZWSv2 <base64EncodedAuthorization>'\n  algorithm: HMACSHA256\n  description: >-\n    iyzico authentication aligns with Basic Auth principles but signs each request.\n    The signature is HMACSHA256(randomKey + uri.path + request.body, secretKey);\n    the authorization string\n    \"apiKey:<apiKey>&randomKey:<randomKey>&signature:<encryptedData>\" is Base64\n    encoded and sent\
  \ as \"IYZWSv2 <base64EncodedAuthorization>\" in the Authorization\n    header.\n  components:\n    apiKey: Unique API key assigned to the merchant account (sandbox keys are prefixed \"sandbox-\").\n    secretKey: Secret key paired with the apiKey; never transmitted, used to sign.\n    randomKey: Per-request nonce (formerly the x-iyzi-rnd random key).\n  additional_headers:\n  - name: x-iyzi-rnd\n    description: Randomly generated per-call value; historically the SHA1 random key.\n  legacy:\n  - name: IYZWS (v1)\n    status: deprecated\n    note: Earlier SHA1-based authorization scheme, superseded by IYZWSv2 (HMACSHA256).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iyzico/refs/heads/main/authentication/iyzico-authentication.yml
summary_line: custom-hmac · 1 scheme
tags:
- Company
- Payments
- FinTech
- Payment Gateway
- Card Payments
- Checkout
- Subscriptions
- Marketplace
- Turkey
- 3D Secure
---
