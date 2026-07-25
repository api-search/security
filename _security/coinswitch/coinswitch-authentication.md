---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Coinswitch Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinSwitch secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CoinSwitch
provider_slug: coinswitch
scheme_count: 2
schemes:
- description: Hex-encoded API key issued from the CoinSwitch PRO account. Sent on every authenticated request in the X-AUTH-APIKEY header.
  in: header
  key_header: X-AUTH-APIKEY
  name: CoinSwitchApiKey
  sources:
  - https://api-trading.coinswitch.co/resources/reference-client
  type: apiKey
- algorithm: ed25519
  description: The client builds signed_message = HTTP_METHOD + url-decoded-path(+query) + epoch, signs it with the account's Ed25519 secret key, and sends the hex signature in X-AUTH-SIGNATURE. X-AUTH-EPOCH is the current Unix millisecond timestamp as a string. The X-AUTH-EPOCH timestamp component was introduced as a security upgrade on 2 Jul 2024; the legacy scheme was phased out after 15 Aug 2024.
  name: CoinSwitchEd25519Signature
  signature_header: X-AUTH-SIGNATURE
  signed_message: METHOD + path + epoch
  sources:
  - https://api-trading.coinswitch.co/resources/reference-client
  timestamp_header: X-AUTH-EPOCH
  type: signature
slug: coinswitch-authentication
source_filename: coinswitch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api-trading.coinswitch.co/get-started/quickstart\ndocs: https://api-trading.coinswitch.co/resources/reference-client\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  signing: ed25519\n  note: >-\n    CoinSwitch PRO uses an API key + Ed25519 secret-key request-signing scheme\n    (not OAuth). Every authenticated request is signed and carries three headers.\nschemes:\n  - name: CoinSwitchApiKey\n    type: apiKey\n    in: header\n    key_header: X-AUTH-APIKEY\n    description: >-\n      Hex-encoded API key issued from the CoinSwitch PRO account. Sent on every\n      authenticated request in the X-AUTH-APIKEY header.\n    sources: [https://api-trading.coinswitch.co/resources/reference-client]\n  - name: CoinSwitchEd25519Signature\n    type: signature\n    algorithm: ed25519\n    signature_header: X-AUTH-SIGNATURE\n    timestamp_header: X-AUTH-EPOCH\n    signed_message: \"METHOD + path + epoch\"\n    description:\
  \ >-\n      The client builds signed_message = HTTP_METHOD + url-decoded-path(+query) +\n      epoch, signs it with the account's Ed25519 secret key, and sends the hex\n      signature in X-AUTH-SIGNATURE. X-AUTH-EPOCH is the current Unix millisecond\n      timestamp as a string. The X-AUTH-EPOCH timestamp component was introduced\n      as a security upgrade on 2 Jul 2024; the legacy scheme was phased out after\n      15 Aug 2024.\n    sources: [https://api-trading.coinswitch.co/resources/reference-client]\nheaders:\n  - X-AUTH-APIKEY\n  - X-AUTH-SIGNATURE\n  - X-AUTH-EPOCH\nnotes: >-\n  No OAuth2/OIDC surface — key-auth provider, so no scopes/ artifact. Reference\n  signing implementations are published for Python, Java, Go, and Node.js.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinswitch/refs/heads/main/authentication/coinswitch-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Cryptocurrency
- Crypto Exchange
- Trading
- Fintech
- Futures
- Spot Trading
- WebSocket
- India
---
