---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Htx Authentication
name_suffix: Authentication
oauth_flows: []
overview: HTX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HTX
provider_slug: htx
scheme_count: 1
schemes:
- docs: https://huobiapi.github.io/docs/spot/v1/en/#signing-api-requests
  in: query
  name: htx-hmac-signature
  parameters:
  - AccessKeyId
  - SignatureMethod
  - SignatureVersion
  - Timestamp
  - Signature
  scheme: hmac-sha256
  signature_version: '2'
  signing: 'Signed string is: HTTP method (GET/POST) + ''\n'' + host + ''\n'' + path + ''\n'' + ASCII-sorted, URL-encoded query parameters. The HMAC-SHA256 digest is signed with the API secret key and Base64-encoded into the Signature parameter.'
  sources:
  - docs
  type: apiKey
slug: htx-authentication
source_filename: htx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://huobiapi.github.io/docs/spot/v1/en/\ndocs: https://www.htx.com/support/360000203002\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\n  notes: >-\n    HTX does not publish an OpenAPI document, so this profile is captured from the\n    developer documentation rather than derived from a spec. Authentication is a\n    per-request HMAC-SHA256 signature (Signature Version 2), not a bearer token or\n    OAuth.\nschemes:\n- name: htx-hmac-signature\n  type: apiKey\n  scheme: hmac-sha256\n  signature_version: '2'\n  in: query\n  parameters:\n    - AccessKeyId          # API key created in Profile > API Management\n    - SignatureMethod      # HmacSHA256\n    - SignatureVersion     # 2\n    - Timestamp            # UTC, format YYYY-MM-DDThh:mm:ss\n    - Signature            # Base64(HMAC-SHA256(secret, canonical request))\n  signing: >-\n    Signed string is: HTTP method (GET/POST) + '\\n' + host + '\\\
  n' + path + '\\n' +\n    ASCII-sorted, URL-encoded query parameters. The HMAC-SHA256 digest is signed\n    with the API secret key and Base64-encoded into the Signature parameter.\n  sources: [docs]\n  docs: https://huobiapi.github.io/docs/spot/v1/en/#signing-api-requests\npermissions:\n  model: per-key\n  scopes: [read-only, trade, withdraw]\n  notes: >-\n    API keys carry granular permissions selected at creation time (read-only,\n    trade). Withdrawal permission is disabled by default and IP allow-listing is\n    supported. This is a key-permission model, not an OAuth scope surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/htx/refs/heads/main/authentication/htx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Technology
- Cryptocurrency
- Crypto Exchange
- Trading
- Digital Assets
- Blockchain
- Financial Services
- Market Data
- WebSocket
---
