---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Musaffa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Musaffa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Musaffa
provider_slug: musaffa
scheme_count: 1
schemes:
- headers:
  - description: Client identifier issued by Musaffa, shared separately with each B2B client.
    name: clientId
    required: true
  - description: Base64(SHA-512(secretKey + time + jsonStringBody)). For the GET /stocks/related/{symbol} operation the stock symbol is signed in place of a JSON body.
    name: token
    required: true
  - description: Request timestamp formatted yyyyMMddHHmmss. The docs state TimeZone = "UTC" but the worked Java example uses ZoneId.of("UTC+5"); the docs are internally inconsistent on this point.
    name: time
    required: true
  - description: application/json
    name: Content-Type
    required: true
  id: musaffa-signed-request
  in: header
  kind: custom-signature
  signature:
    algorithm: SHA-512
    canonical_string: secretKey + time + jsonStringBody
    encoding: base64
    replay_window_seconds: 5
    replay_window_source: Errors section — "Gives a 'Time expired' error if the token time exceeds 5 seconds" (HTTP 400).
  standard: none
slug: musaffa-authentication
source_filename: musaffa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://api.musaffa.com/\ndocs: https://api.musaffa.com/\nname: Musaffa B2B API authentication\nsummary: >-\n  Musaffa does not use OAuth, OpenID Connect or a bearer API key. Each B2B client is issued a\n  clientId and a secretKey out of band (there is no self-service key issuance), and every request\n  carries a per-request signature computed over the secret, a UTC timestamp and the exact request\n  body. The scheme is a custom HMAC-style request signature, not a static credential.\nschemes:\n- id: musaffa-signed-request\n  kind: custom-signature\n  in: header\n  standard: none\n  headers:\n  - name: clientId\n    description: Client identifier issued by Musaffa, shared separately with each B2B client.\n    required: true\n  - name: token\n    description: >-\n      Base64(SHA-512(secretKey + time + jsonStringBody)). For the GET /stocks/related/{symbol}\n      operation the stock symbol is signed in place of a JSON body.\n\
  \    required: true\n  - name: time\n    description: >-\n      Request timestamp formatted yyyyMMddHHmmss. The docs state TimeZone = \"UTC\" but the worked\n      Java example uses ZoneId.of(\"UTC+5\"); the docs are internally inconsistent on this point.\n    required: true\n  - name: Content-Type\n    description: application/json\n    required: true\n  signature:\n    algorithm: SHA-512\n    encoding: base64\n    canonical_string: secretKey + time + jsonStringBody\n    replay_window_seconds: 5\n    replay_window_source: >-\n      Errors section — \"Gives a 'Time expired' error if the token time exceeds 5 seconds\" (HTTP 400).\ncredential_issuance:\n  self_service: false\n  method: sales\n  note: >-\n    \"Musaffa will provide a secret key and a client ID to every B2B client\" — credentials are issued\n    through the demo / schedule-a-call flow on https://musaffa.com/for-business/. There is no\n    developer signup that yields API credentials.\noauth2: false\nopenid_connect: false\n\
  mutual_tls: false\nscopes: none\nnotes:\n- The same clientId/token/time header triple is used in BOTH directions — Musaffa signs its outbound\n  webhook deliveries with the identical scheme, so a consumer can verify inbound webhooks by\n  recomputing Base64(SHA-512(secretKey + time + body)).\n- Published example credential values in the docs are placeholders, not live keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musaffa/refs/heads/main/authentication/musaffa-authentication.yml
summary_line: 1 scheme
tags:
- Islamic Finance
- Shariah Compliance
- Halal Investing
- Stock Screening
- Financial Data
- ETFs
- Market Data
- Fintech
- Investing
- Compliance
- Zakat
- Company
---
