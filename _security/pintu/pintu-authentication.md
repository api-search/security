---
api_key_in:
- payload
auth_types:
- apiKey
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Pintu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pintu secures its APIs with apiKey and hmac across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pintu
provider_slug: pintu
scheme_count: 1
schemes:
- channels:
    private: requires the WebSocket channel subscription routine before streaming
    public: no subscription handshake required
  description: Every request (HTTP or WebSocket) is wrapped in a signed envelope. The caller supplies an API key and computes an HMAC-SHA256 signature over the request payload using their API secret; the resulting hex string is placed in the wrapper's signature field. A place-order request wrapper carries request_id, method, api_key, params, timestamp, and signature.
  fields:
    api_key: the partner's issued API key
    method: the operation being invoked
    params: operation-specific parameters
    request_id: unique client-generated request identifier
    signature: HMAC-SHA256(secret, payload) as hex
    timestamp: request timestamp (replay protection)
  in: payload
  key_field: api_key
  name: PintuHMAC
  scheme: hmac-sha256
  signature_field: signature
  type: apiKey
slug: pintu-authentication
source_filename: pintu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pintu.pro/\ndocs: https://docs.pintu.pro/\nsummary:\n  types: [apiKey, hmac]\n  api_key_in: [payload]\n  oauth2_flows: []\n  transports: [http, websocket]\nschemes:\n- name: PintuHMAC\n  type: apiKey\n  scheme: hmac-sha256\n  in: payload\n  key_field: api_key\n  signature_field: signature\n  description: >-\n    Every request (HTTP or WebSocket) is wrapped in a signed envelope. The\n    caller supplies an API key and computes an HMAC-SHA256 signature over the\n    request payload using their API secret; the resulting hex string is placed\n    in the wrapper's signature field. A place-order request wrapper carries\n    request_id, method, api_key, params, timestamp, and signature.\n  fields:\n    request_id: unique client-generated request identifier\n    method: the operation being invoked\n    api_key: the partner's issued API key\n    params: operation-specific parameters\n    timestamp: request timestamp (replay\
  \ protection)\n    signature: HMAC-SHA256(secret, payload) as hex\n  channels:\n    public: no subscription handshake required\n    private: requires the WebSocket channel subscription routine before streaming\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pintu/refs/heads/main/authentication/pintu-authentication.yml
summary_line: apiKey/hmac · 1 scheme
tags:
- Company
- Cryptocurrency
- Crypto Exchange
- Trading
- Fintech
- Digital Assets
- Web3
- Indonesia
- WebSocket
- Institutional Trading
---
