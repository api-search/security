---
api_key_in:
- sdk-configuration
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Doorstep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doorstep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doorstep
provider_slug: doorstep
scheme_count: 1
schemes:
- configured_via: DoorstepAI.setApiKey(key:)
  format: JWT
  guidance: Store API keys securely using environment variables or a secure configuration service; never hardcode API keys in production builds. Invalid keys surface as errors on the async initialization/start calls (wrap in do/catch).
  name: apiKey
  platform_examples:
  - call: 'DoorstepAI.setApiKey(key: "<JWT>")'
    platform: ios
  - call: DoorstepAI.setAPIKey("your_api_key_here")
    platform: android
  type: apiKey
slug: doorstep-authentication
source_filename: doorstep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.doorstep.ai/iOS/using\ndocs: https://docs.doorstep.ai/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - sdk-configuration\n  token_format: JWT\n  oauth2_flows: []\n  note: >-\n    Doorstep exposes a client-side mobile tracking SDK (Dropoff SDK), not a public\n    REST API. Authentication is a single API key (a JWT) provisioned by Doorstep and\n    set programmatically in the SDK before tracking begins. There is no OpenAPI spec,\n    OAuth flow, or documented scope surface.\nschemes:\n- name: apiKey\n  type: apiKey\n  format: JWT\n  configured_via: DoorstepAI.setApiKey(key:)\n  platform_examples:\n  - platform: ios\n    call: 'DoorstepAI.setApiKey(key: \"<JWT>\")'\n  - platform: android\n    call: 'DoorstepAI.setAPIKey(\"your_api_key_here\")'\n  guidance: >-\n    Store API keys securely using environment variables or a secure configuration\n    service; never hardcode API keys in production builds. Invalid keys\
  \ surface as\n    errors on the async initialization/start calls (wrap in do/catch).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doorstep/refs/heads/main/authentication/doorstep-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Delivery
- Last-Mile Logistics
- Indoor Positioning
- Location Tracking
- Mobile SDK
- Delivery Tracking
- Fraud Prevention
- Proof of Delivery
---
