---
api_key_in: []
auth_types:
- jwt-signed-webhook
- ble-pairing
description: ''
kind: authentication
layout: security
method: searched
name: Flic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flic secures its APIs with jwt-signed-webhook and ble-pairing across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Flic
provider_slug: flic
scheme_count: 2
schemes:
- algorithm: ES256
  direction: inbound-webhook
  key_type: ECDSA P-256
  name: cloud-buttons-jwt
  scheme: JWT
  sources:
  - asyncapi/flic-cloud-buttons-webhooks.yml
  type: jws
  verification: The receiving endpoint verifies the ES256-signed JWT using Flic's public key (published in JWK/PEM/DER/raw). Claims carry the button uuid, serial, battery, pressedAt, and click type.
- direction: sdk-to-button
  name: ble-pairing
  scheme: Bluetooth Low Energy
  sources:
  - packages/flic-packages.yml
  type: device-pairing
  verification: flic2lib (iOS/Android/C/Linux/Windows) establishes a paired, encrypted BLE session with the button; there is no server-side token exchange.
slug: flic-authentication
source_filename: flic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/50ButtonsEach/flic-cloud-buttons-documentation\ndocs: https://github.com/50ButtonsEach/flic2-documentation\nsummary:\n  types: [jwt-signed-webhook, ble-pairing]\n  note: >-\n    Flic has no OAuth/REST API-key surface. Two authentication models are in\n    play: (1) SDK/protocol access to buttons is authenticated via Bluetooth Low\n    Energy pairing between the Flic 2 button and the host app/hub (the pairing\n    identity is what the flic2lib SDKs establish); (2) Cloud Buttons webhook\n    deliveries are authenticated to the receiver by a signed JWT.\nschemes:\n  - name: cloud-buttons-jwt\n    type: jws\n    scheme: JWT\n    algorithm: ES256\n    key_type: ECDSA P-256\n    direction: inbound-webhook\n    verification: >-\n      The receiving endpoint verifies the ES256-signed JWT using Flic's public\n      key (published in JWK/PEM/DER/raw). Claims carry the button uuid, serial,\n      battery, pressedAt,\
  \ and click type.\n    sources: [asyncapi/flic-cloud-buttons-webhooks.yml]\n  - name: ble-pairing\n    type: device-pairing\n    scheme: Bluetooth Low Energy\n    direction: sdk-to-button\n    verification: >-\n      flic2lib (iOS/Android/C/Linux/Windows) establishes a paired, encrypted BLE\n      session with the button; there is no server-side token exchange.\n    sources: [packages/flic-packages.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flic/refs/heads/main/authentication/flic-authentication.yml
summary_line: jwt-signed-webhook/ble-pairing · 2 schemes
tags:
- Company
- Smart Buttons
- IoT
- Smart Home
- Bluetooth
- Webhooks
- SDK
- Hardware
---
