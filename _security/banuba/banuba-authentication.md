---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Banuba Authentication
name_suffix: Authentication
oauth_flows: []
overview: Banuba declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Banuba
provider_slug: banuba
scheme_count: 3
schemes:
- applies_to:
  - Face AR SDK
  - WebAR SDK
  - Video Editor SDK
  - Photo Editor SDK
  - AR Cloud SDK
  - AI Talking Photo SDK
  expiry: 14 days (demo) / prepaid licence period (commercial); one-month watermark grace, then the SDK stops (see lifecycle/)
  how: A generated .txt token unique to each client, passed to the SDK at initialisation (e.g. the token string in BanubaClientToken.swift / the `clientToken` argument of the WebAR Player). It activates the licensed feature set; it is validated on-device and is not a bearer credential for an HTTP API.
  id: client_token
  obtain: 'Demo token: request via the website form (https://www.banuba.com/facear-sdk/face-filters#form) or a sales manager — valid 14 days. Commercial token: issued by the account manager after payment, valid for the prepaid period.'
  storage_guidance: store server-side so renewals do not require a store release; never ship demo tokens in live apps
  type: licence-token
- applies_to:
  - TINT virtual try-on widget (<tint-vto>)
  how: The embeddable widget is configured with a merchantId or a publishableKey (query/attribute) plus an optional token and short code `q`; it calls the Tint public API (api.tintvto.com/api/v1/public) on the merchant's behalf. The key format and the API's server-side auth are undocumented; merchants get them from the app.tintvto.com admin.
  id: tint_publishable_key
  type: publishable-key
- applies_to:
  - app.tintvto.com admin
  how: Merchant sign-in via accounts.tintvto.com (Clerk-hosted); not a developer credential.
  id: tint_admin_session
  type: session (Clerk)
slug: banuba-authentication
source_filename: banuba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://docs.banuba.com/far-sdk/tutorials/capabilities/token_management, https://docs.banuba.com/far-sdk/tutorials/development/basic_integration,\n  https://www.banuba.com/banuba-pricing-face-ar-sdk (FAQ \"Where can I find my client token?\"), https://tintvto.com/ (widget parameters),\n  https://github.com/Banuba/BanubaGenAIVideos-iOS (AI Talking Photo SDK README) — read 2026-09-17.\ndocs: https://docs.banuba.com/far-sdk/tutorials/capabilities/token_management\nsurface: sdk\nnote: >-\n  Banuba publishes no OpenAPI, so nothing here is a securityScheme in the OpenAPI sense. What the docs document is\n  SDK licence activation: every SDK (Face AR, WebAR, Video Editor, Photo Editor, AR Cloud) is initialised with a\n  per-customer client token issued by Banuba sales / the account manager. The AI Talking Photo API — the one hosted\n  API Banuba markets — uses \"a Banuba trial token\" but its API docs are only available on request\
  \ through Support,\n  so its HTTP auth mechanism is not publicly documented and is NOT described here.\nschemes:\n  - id: client_token\n    type: licence-token\n    applies_to: [Face AR SDK, WebAR SDK, Video Editor SDK, Photo Editor SDK, AR Cloud SDK, AI Talking Photo SDK]\n    how: >-\n      A generated .txt token unique to each client, passed to the SDK at initialisation (e.g. the token string in\n      BanubaClientToken.swift / the `clientToken` argument of the WebAR Player). It activates the licensed feature\n      set; it is validated on-device and is not a bearer credential for an HTTP API.\n    obtain: >-\n      Demo token: request via the website form (https://www.banuba.com/facear-sdk/face-filters#form) or a sales\n      manager — valid 14 days. Commercial token: issued by the account manager after payment, valid for the prepaid period.\n    expiry: 14 days (demo) / prepaid licence period (commercial); one-month watermark grace, then the SDK stops (see lifecycle/)\n    storage_guidance:\
  \ store server-side so renewals do not require a store release; never ship demo tokens in live apps\n  - id: tint_publishable_key\n    type: publishable-key\n    applies_to: [TINT virtual try-on widget (<tint-vto>)]\n    how: >-\n      The embeddable widget is configured with a merchantId or a publishableKey (query/attribute) plus an optional\n      token and short code `q`; it calls the Tint public API (api.tintvto.com/api/v1/public) on the merchant's behalf.\n      The key format and the API's server-side auth are undocumented; merchants get them from the app.tintvto.com admin.\n  - id: tint_admin_session\n    type: session (Clerk)\n    applies_to: [app.tintvto.com admin]\n    how: Merchant sign-in via accounts.tintvto.com (Clerk-hosted); not a developer credential.\noauth: false\napi_keys: false\nmutual_tls: false\ngated:\n  - surface: AI Talking Photo API\n    note: HTTP auth undocumented publicly; \"request access for AI Talking Photo specific docs via Support\" (BanubaGenAIVideos-iOS\
  \ README).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banuba/refs/heads/main/authentication/banuba-authentication.yml
summary_line: 3 schemes
tags:
- AR
- Augmented Reality
- Beauty
- Face Recognition
- Facial
- SDK
- Video
---
