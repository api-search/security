---
api_key_in:
- hmac-seed
auth_types:
- hmac
description: Authentication profile for the Vauld Enterprise API, captured from the published API reference at docs.vauld.com. Vauld does not publish an OpenAPI document; this profile was captured from the HTML docs.
kind: authentication
layout: security
method: searched
name: Vauld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vauld secures its APIs with hmac across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vauld
provider_slug: vauld
scheme_count: 1
schemes:
- credentials:
  - name: APIKey
    obtain: Contact Vauld (email in docs) for production API keys; a test API key is provided in the docs per API section
  - name: orgID
    obtain: Organisation ID issued by Vauld, sent in every request body
  description: 'HMAC-SHA256 request signing. The JSON request body is serialized to URI format (key=value pairs joined with ''&''), then an HMAC hash is computed with the SHA-256 algorithm using the organisation''s APIKey as the seed. The hash, hex-encoded, is sent in the `hmac` request header alongside `Content-Type: application/json`. Every request body also carries the organisation''s `orgID`.'
  headers:
  - name: hmac
    value: HMAC-SHA256 hash of the URI-encoded payload, hex-encoded
  - name: Content-Type
    value: application/json
  name: hmac
  sources:
  - https://docs.vauld.com/
  type: custom-hmac
slug: vauld-authentication
source_filename: vauld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vauld.com/\ndocs: https://docs.vauld.com/\ndescription: >-\n  Authentication profile for the Vauld Enterprise API, captured from the\n  published API reference at docs.vauld.com. Vauld does not publish an\n  OpenAPI document; this profile was captured from the HTML docs.\nsummary:\n  types: [hmac]\n  api_key_in: [hmac-seed]\n  oauth2_flows: []\nschemes:\n  - name: hmac\n    type: custom-hmac\n    description: >-\n      HMAC-SHA256 request signing. The JSON request body is serialized to\n      URI format (key=value pairs joined with '&'), then an HMAC hash is\n      computed with the SHA-256 algorithm using the organisation's APIKey\n      as the seed. The hash, hex-encoded, is sent in the `hmac` request\n      header alongside `Content-Type: application/json`. Every request\n      body also carries the organisation's `orgID`.\n    headers:\n      - name: hmac\n        value: HMAC-SHA256 hash of the URI-encoded\
  \ payload, hex-encoded\n      - name: Content-Type\n        value: application/json\n    credentials:\n      - name: APIKey\n        obtain: Contact Vauld (email in docs) for production API keys; a test API key is provided in the docs per API section\n      - name: orgID\n        obtain: Organisation ID issued by Vauld, sent in every request body\n    sources: [https://docs.vauld.com/]\nnotes: >-\n  No OAuth2, OpenID Connect, or bearer-token surface is documented. All\n  documented operations are HTTP POST with the HMAC header. The docs ship\n  a JavaScript (CryptoJS) example of the signing routine.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vauld/refs/heads/main/authentication/vauld-authentication.yml
summary_line: hmac · 1 scheme
tags:
- Company
- Crypto
- Lending
- Borrowing
- Trading
- Wallets
- KYC
- Fintech
- India
- Singapore
---
