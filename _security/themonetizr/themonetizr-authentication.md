---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Themonetizr Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheMonetizr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TheMonetizr
provider_slug: themonetizr
scheme_count: 1
schemes:
- description: 'The Monetizr Campaigns API authenticates with a per-game API key sent as an HTTP Bearer token (Authorization: Bearer <apiKey>). The key is provisioned per game/application in the Monetizr console and configured in the SDK MonetizrSettings.'
  name: bearerAuth
  scheme: bearer
  sources:
  - The-Monetizr-Campaigns-Unity-SDK/NetworkingUtils.cs
  type: http
slug: themonetizr-authentication
source_filename: themonetizr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: The-Monetizr-Campaigns-Unity-SDK (Assets/MonetizrCampaigns/Scripts/Networking/NetworkingUtils.cs, MonetizrHttpClient.cs)\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      The Monetizr Campaigns API authenticates with a per-game API key sent as an\n      HTTP Bearer token (Authorization: Bearer <apiKey>). The key is provisioned\n      per game/application in the Monetizr console and configured in the SDK\n      MonetizrSettings.\n    sources:\n      - The-Monetizr-Campaigns-Unity-SDK/NetworkingUtils.cs\ncontext_headers:\n  - name: player-id\n    description: Device/player identifier used for campaign targeting and reward attribution.\n  - name: ad-id\n    description: Platform advertising identifier (IDFA/GAID).\n  - name: sdk-version\n    description: Monetizr SDK version string.\n  - name:\
  \ os-group\n    description: Coarse OS group of the requesting device.\n  - name: device-group\n    description: Coarse device-size/class group.\nnotes:\n  - No OAuth2 or OpenID Connect surface is present; auth is a static per-game Bearer API key.\n  - The provider publishes no OpenAPI/security scheme document; this profile is derived from the first-party Unity SDK source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/themonetizr/refs/heads/main/authentication/themonetizr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Advertising
- Gaming
- In-Game Advertising
- Monetization
- Mobile
- Rewards
- Ad Tech
- Programmatic
- Unity
---
