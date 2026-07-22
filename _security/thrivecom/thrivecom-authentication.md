---
api_key_in:
- body
- path
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Thrivecom Authentication
name_suffix: Authentication
oauth_flows: []
overview: RingCaptcha (ThriveCom) secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RingCaptcha (ThriveCom)
provider_slug: thrivecom
scheme_count: 3
schemes:
- description: Per-application public key that identifies the RingCaptcha app; embedded in the URL path as /{app_key}/{endpoint}.
  in: path
  name: app_key
  sources:
  - ringcaptcha-node/lib/RingCaptcha.js
  - ringcaptcha-python/lib/Ringcaptcha.py
  type: apiKey
- description: Public application API key sent as a form field on most operations.
  in: body
  name: api_key
  parameter: api_key
  sources:
  - ringcaptcha-node/lib/Config.js
  type: apiKey
- description: Server-side secret key sent as a form field on secured operations (verify, captcha, sms) to authorize the request; never exposed client-side.
  in: body
  name: secret_key
  parameter: secret_key
  sources:
  - ringcaptcha-python/lib/Ringcaptcha.py
  - ringcaptcha-node/lib/Config.js
  type: apiKey
slug: thrivecom-authentication
source_filename: thrivecom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: 'https://github.com/ringcaptcha (official SDK source: ringcaptcha-node, ringcaptcha-python)'\ndocs: https://my.ringcaptcha.com/docs/web\nsummary:\n  types: [apiKey]\n  api_key_in: [body, path]\n  oauth2_flows: []\n  notes: >-\n    RingCaptcha uses static API-key credentials, not OAuth. Every request is\n    authenticated with a triplet of keys issued per application in the\n    dashboard: api_key and secret_key sent as form parameters, and app_key\n    embedded in the request path (/{app_key}/{endpoint}). Requests are\n    application/x-www-form-urlencoded over HTTPS to api.ringcaptcha.com.\nschemes:\n  - name: app_key\n    type: apiKey\n    in: path\n    description: >-\n      Per-application public key that identifies the RingCaptcha app; embedded\n      in the URL path as /{app_key}/{endpoint}.\n    sources: [ringcaptcha-node/lib/RingCaptcha.js, ringcaptcha-python/lib/Ringcaptcha.py]\n  - name: api_key\n    type: apiKey\n\
  \    in: body\n    parameter: api_key\n    description: Public application API key sent as a form field on most operations.\n    sources: [ringcaptcha-node/lib/Config.js]\n  - name: secret_key\n    type: apiKey\n    in: body\n    parameter: secret_key\n    description: >-\n      Server-side secret key sent as a form field on secured operations\n      (verify, captcha, sms) to authorize the request; never exposed client-side.\n    sources: [ringcaptcha-python/lib/Ringcaptcha.py, ringcaptcha-node/lib/Config.js]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivecom/refs/heads/main/authentication/thrivecom-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Two-Factor Authentication
- Phone Verification
- One-Time Passcode
- SMS
- Voice
- Fraud Prevention
- Identity Verification
- Authentication
---
