---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kgen Authentication
name_suffix: Authentication
oauth_flows: []
overview: KGeN secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KGeN
provider_slug: kgen
scheme_count: 2
schemes:
- applies_to: /s2s/* endpoints (session creation, loyalty rewardable-events)
  in: header
  keys:
  - x-client-id
  - x-client-secret
  name: server-to-server
  sources:
  - docs.kgen.io Tech Integration
  type: apiKey
- applies_to: /fe/* endpoints (tournaments, wallet, rewards, statistics)
  in: header
  key: user-jwt-token
  name: user-jwt
  sources:
  - docs.kgen.io Tech Integration
  type: apiKey
slug: kgen-authentication
source_filename: kgen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kgen.io/docs/Esport%20Protocol%20V1/Tech%20integration/user-session\ndocs: https://docs.kgen.io/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    KGeN Economy Protocols use two distinct credential styles. Server-to-server\n    (/s2s/*) endpoints authenticate with a client id + client secret pair sent as\n    request headers. Front-end (/fe/*) endpoints authenticate with a per-user JWT\n    sent in the user-jwt-token header, obtained via the phone-number OTP flow. No\n    OAuth 2.0 / OpenID Connect surface is documented.\nschemes:\n  - name: server-to-server\n    type: apiKey\n    in: header\n    keys:\n      - x-client-id      # your unique client identifier\n      - x-client-secret  # your client secret\n    applies_to: /s2s/* endpoints (session creation, loyalty rewardable-events)\n    sources: [docs.kgen.io Tech Integration]\n  - name: user-jwt\n    type: apiKey\n  \
  \  in: header\n    key: user-jwt-token   # user's JWT for authentication\n    applies_to: /fe/* endpoints (tournaments, wallet, rewards, statistics)\n    sources: [docs.kgen.io Tech Integration]\nuser_authentication:\n  method: phone-number OTP\n  flow:\n    - POST /fe/users/auth/otp/register   # request OTP; returns authCode + isNewUser\n    - POST /fe/users/auth/otp/resend     # resend OTP\n    - POST /fe/users/auth/otp/verify     # verify OTP; links custodial wallet to KGeN wallet\n  request_headers:\n    - Content-Type: application/json\n    - user-jwt-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kgen/refs/heads/main/authentication/kgen-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Marketplaces
- Gaming
- Esports
- Loyalty
- Rewards
- Web3
- AI Data
- Developer API
---
