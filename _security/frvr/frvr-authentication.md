---
api_key_in: []
auth_types:
- oauth2-jwt
- platform-federated
- anonymous
description: ''
kind: authentication
layout: security
method: searched
name: Frvr Authentication
name_suffix: Authentication
oauth_flows: []
overview: FRVR secures its APIs with oauth2-jwt, platform-federated, and anonymous across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FRVR
provider_slug: frvr
scheme_count: 0
schemes: []
slug: frvr-authentication
source_filename: frvr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.frvr.com/modules/auth/\ndocs: https://docs.frvr.com/modules/auth/\nsummary:\n  types: [oauth2-jwt, platform-federated, anonymous]\n  token_format: JWT bearer (FRVR.auth.getAccessToken())\n  scheme_surface: SDK-mediated (no public REST securityScheme; auth is handled by the FRVR JS SDK)\nmodel: >-\n  FRVR.auth authenticates the current player against FRVR's backend — either with a\n  FRVR account, a platform provider (Facebook, Google Play, Apple, ...), or\n  anonymously. The SDK auto-attempts login in priority order: cached token from\n  storage (if valid) -> platform credentials from the host channel -> anonymous\n  sign-in (if enabled). It returns a JWT access token for backend calls, which the\n  SDK refreshes in the background at ~60% of its TTL.\nmethods:\n  - name: FRVR.auth.isLoggedIn()\n    purpose: Confirm an active session.\n  - name: FRVR.auth.getAccessToken()\n    purpose: Return the JWT for authenticated\
  \ backend calls.\n  - name: FRVR.auth.getFRVRID()\n    purpose: Retrieve the player's stable FRVR identifier.\n  - name: FRVR.auth.loginToFRVR({ platform, credentials })\n    purpose: Explicit login with a FRVR account or a platform provider.\n  - name: FRVR.auth.registerOnFRVR({ email, password, firstName, lastName }, autoLogin)\n    purpose: Register a new FRVR account and optionally auto-login.\n  - name: FRVR.auth.addStatusChangeListener(cb)\n    purpose: Subscribe to auth status changes ({ isLoggedIn, platform }).\nproviders:\n  - frvr\n  - facebook-instant\n  - google-play\n  - apple\n  - anonymous\nnotes: >-\n  Anonymous sessions still persist a stable ID and can be upgraded to a real\n  account later. Configure with FRVR.config.auth = {} to use the channel's default\n  provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frvr/refs/heads/main/authentication/frvr-authentication.yml
summary_line: oauth2-jwt/platform-federated/anonymous · 0 schemes
tags:
- Company
- Gaming
- Games
- Game Development
- SDK
- HTML5
- Instant Games
- Monetization
- Ads
- In-App Purchases
---
