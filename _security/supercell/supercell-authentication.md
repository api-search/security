---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Supercell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supercell secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Supercell
provider_slug: supercell
scheme_count: 1
schemes:
- applies_to:
  - https://api.clashofclans.com/v1
  - https://api.clashroyale.com/v1
  - https://api.brawlstars.com/v1
  bearer_format: JWT
  description: 'A long-lived JWT API token created in the game''s developer portal and passed as "Authorization: Bearer <token>". Each token is bound to a set of allowed (whitelisted) IP addresses at creation time; requests from other IPs are rejected. All endpoints are read-only.'
  name: bearerAuth
  scheme: bearer
  token_management:
  - https://developer.clashofclans.com
  - https://developer.clashroyale.com
  - https://developer.brawlstars.com
  type: http
slug: supercell-authentication
source_filename: supercell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.clashofclans.com/#/documentation\nnote: >-\n  No public OpenAPI is fetchable (the API hosts require auth and the portals are SPAs), so\n  this profile is captured from the documented and live-verified auth mechanism rather than\n  derived from a spec. All three Supercell game APIs (Clash of Clans, Clash Royale, Brawl\n  Stars) share one identical model. Verified live: unauthenticated calls to each api.*/v1\n  host return HTTP 403 {\"reason\":\"accessDenied\",\"message\":\"Missing authorization\"}.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  ip_whitelisting: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    A long-lived JWT API token created in the game's developer portal and passed as\n    \"Authorization: Bearer <token>\". Each token is bound to a set of allowed (whitelisted)\n    IP addresses at creation time;\
  \ requests from other IPs are rejected. All endpoints are\n    read-only.\n  applies_to:\n  - https://api.clashofclans.com/v1\n  - https://api.clashroyale.com/v1\n  - https://api.brawlstars.com/v1\n  token_management:\n  - https://developer.clashofclans.com\n  - https://developer.clashroyale.com\n  - https://developer.brawlstars.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supercell/refs/heads/main/authentication/supercell-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Gaming
- Mobile Games
- Video Games
- Game Data
- Developer API
- Leaderboards
- Esports
---
