---
api_key_in:
- body
auth_types:
- apiKey
description: Bitmain's public developer surface is the Antpool mining-pool API. It uses a signed API-key model rather than OAuth. Each operator is issued an API "Key" and "Secret"; every private request must include the user id, the API key, an incrementing integer nonce, and a signature. The signature is an HMAC-SHA256 hex digest (uppercased) of the message `userId + apiKey + nonce` computed with the operator's API secret. There is no OAuth authorization server, no scopes, and no OpenID Connect.
kind: authentication
layout: security
method: searched
name: Bitmain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitmain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitmain
provider_slug: bitmain
scheme_count: 1
schemes:
- description: Signed request authentication. Send `key` (API key), `nonce` (increasing integer), and `signature` (HMAC-SHA256 of userId+key+nonce, keyed by the API secret, hex, uppercased) as request parameters on every private call.
  in: body
  name: antpool-signature
  parameters:
  - key
  - nonce
  - signature
  signature_algorithm: HMAC-SHA256
  signature_message: userId + apiKey + nonce
  sources:
  - https://www.antpool.com/userApiGuide
  type: apiKey
slug: bitmain-authentication
source_filename: bitmain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.antpool.com/userApiGuide\ndocs: https://www.antpool.com/userApiGuide\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - body\n  signature: HMAC-SHA256\ndescription: >-\n  Bitmain's public developer surface is the Antpool mining-pool API. It uses a\n  signed API-key model rather than OAuth. Each operator is issued an API \"Key\"\n  and \"Secret\"; every private request must include the user id, the API key, an\n  incrementing integer nonce, and a signature. The signature is an\n  HMAC-SHA256 hex digest (uppercased) of the message `userId + apiKey + nonce`\n  computed with the operator's API secret. There is no OAuth authorization\n  server, no scopes, and no OpenID Connect.\nschemes:\n- name: antpool-signature\n  type: apiKey\n  in: body\n  description: >-\n    Signed request authentication. Send `key` (API key), `nonce` (increasing\n    integer), and `signature` (HMAC-SHA256 of userId+key+nonce, keyed by the API\n\
  \    secret, hex, uppercased) as request parameters on every private call.\n  parameters:\n  - key\n  - nonce\n  - signature\n  signature_algorithm: HMAC-SHA256\n  signature_message: userId + apiKey + nonce\n  sources:\n  - https://www.antpool.com/userApiGuide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmain/refs/heads/main/authentication/bitmain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Technology
- Cryptocurrency
- Bitcoin
- Mining
- Mining Pool
- Hardware
- Blockchain
---
