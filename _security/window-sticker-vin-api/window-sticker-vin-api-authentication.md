---
anonymous_access: false
api_key_in: []
api_specs:
- filename: window-sticker-vin-api-openapi.yml
  format: yaml
  label: Window Sticker VIN API
  slug: window-sticker-vin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/window-sticker-vin-api/refs/heads/main/openapi/window-sticker-vin-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Window Sticker Vin Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Window Sticker VIN API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Window Sticker VIN API
provider_slug: window-sticker-vin-api
scheme_count: 0
schemes: []
slug: window-sticker-vin-api-authentication
source_filename: window-sticker-vin-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: derived\nsource: >-\n  openapi/window-sticker-vin-api-openapi.yml (no securitySchemes, no security requirement)\n  cross-checked against https://windowsticker.org/api-docs\nsummary: >-\n  Public, keyless API. The OpenAPI declares no securitySchemes and no security requirement,\n  and the docs confirm it: \"Free, keyless, CORS-enabled. No registration and no tiers.\"\n  Both operations are anonymous GET requests. There is nothing to authenticate.\nschemes: []\nrequires_auth: false\npublic: true\ncors:\n  enabled: true\n  note: Documented as CORS-enabled for browser-side use.\nnotes: >-\n  No API key, no OAuth, no OpenID Connect, no mTLS. No /.well-known/oauth-authorization-server\n  or /.well-known/openid-configuration is served (both 404), consistent with a keyless service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/window-sticker-vin-api/refs/heads/main/authentication/window-sticker-vin-api-authentication.yml
summary_line: 0 schemes
tags:
- Automotive
- Vehicle Data
- VIN Decoding
- Monroney
- Window sticker
- Government open data
- Auto Retail
- Dealer tooling
---
