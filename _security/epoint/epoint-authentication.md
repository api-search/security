---
api_key_in:
- body
auth_types:
- custom-signature
description: ''
kind: authentication
layout: security
method: searched
name: Epoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epoint secures its APIs with custom-signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Epoint
provider_slug: epoint
scheme_count: 1
schemes:
- description: Each API request sends two form-encoded POST parameters. `data` is the Base64-encoded JSON body (which itself carries the merchant `public_key`). `signature` is base64_encode(sha1(private_key + data + private_key, raw=1)), proving the merchant holds the private key and the payload was not tampered with. The same signature scheme is used to verify inbound callbacks.
  name: EpointSignature
  parameters:
    data:
      description: Base64-encoded JSON request payload.
      location: form-body
    public_key:
      description: Merchant identifier issued at registration (e.g. i000000001).
      location: json-body
    signature:
      description: Base64(SHA1(private_key + data + private_key)) integrity/auth signature.
      location: form-body
  private_key:
    description: Never transmitted; used only to compute/verify the signature.
    handling: server-side-secret
  scheme: data+signature
  type: custom
slug: epoint-authentication
source_filename: epoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.epoint.az/en/authentication\ndocs: https://developer.epoint.az/en/authentication\nsummary:\n  types:\n  - custom-signature\n  api_key_in:\n  - body\n  oauth2_flows: []\n  note: >-\n    Epoint does not use OAuth or a bearer token. Every request is authenticated\n    with a merchant public_key plus an HMAC-style request signature over the\n    Base64-encoded JSON payload, keyed by the merchant private_key.\nschemes:\n- name: EpointSignature\n  type: custom\n  scheme: data+signature\n  description: >-\n    Each API request sends two form-encoded POST parameters. `data` is the\n    Base64-encoded JSON body (which itself carries the merchant `public_key`).\n    `signature` is base64_encode(sha1(private_key + data + private_key, raw=1)),\n    proving the merchant holds the private key and the payload was not tampered\n    with. The same signature scheme is used to verify inbound callbacks.\n  parameters:\n    public_key:\n\
  \      location: json-body\n      description: Merchant identifier issued at registration (e.g. i000000001).\n    data:\n      location: form-body\n      description: Base64-encoded JSON request payload.\n    signature:\n      location: form-body\n      description: Base64(SHA1(private_key + data + private_key)) integrity/auth signature.\n  private_key:\n    handling: server-side-secret\n    description: Never transmitted; used only to compute/verify the signature.\ncallback_verification:\n  method: same-signature\n  description: >-\n    Inbound callbacks to the merchant result_url carry `data` + `signature`.\n    The merchant recomputes the signature with its private_key and compares to\n    confirm authenticity before decoding `data`.\ntracing:\n  request_id_field: trace_id\n  response_header: X-Request-ID\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epoint/refs/heads/main/authentication/epoint-authentication.yml
summary_line: custom-signature · 1 scheme
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- E-commerce
- Card Payments
- Azerbaijan
- Apple Pay
- Google Pay
- Digital Wallet
---
