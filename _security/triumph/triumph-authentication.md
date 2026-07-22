---
api_key_in: []
auth_types:
- sdk-credentials
description: ''
kind: authentication
layout: security
method: searched
name: Triumph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Triumph secures its APIs with sdk-credentials across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Triumph
provider_slug: triumph
scheme_count: 5
schemes:
- description: Per-game identifier issued in the Triumph developer dashboard (game's "go live" tab). Passed to Triumph.configure(id:) in Swift or set on TriumphUnityNativeMethods.gameId in Unity. An empty gameId runs the SDK in sandbox mode.
  name: gameId
  source: https://docs.triumpharcade.com/triumph-sdk/import-triumph.md
  type: sdk-configuration
- description: Merchant identifier set alongside gameId in the Unity TriumphUnityNativeMethods integration.
  name: merchantId
  source: https://docs.triumpharcade.com/triumph-sdk/import-triumph.md
  type: sdk-configuration
- description: Apple Push Notification Service (APNs) key created in the Apple Developer account and uploaded (with its Key ID) under Settings > Apple Keys in the Triumph dashboard; used to notify players of tournament results.
  name: apple-apns-key
  source: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md
  type: platform-key
- description: Apple DeviceCheck key created in the Apple Developer account and uploaded to the Triumph dashboard; used to verify submitted scores come from a real device.
  name: apple-devicecheck-key
  source: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md
  type: platform-key
- description: Apple Developer Team ID recorded in the Triumph dashboard alongside the APNs and DeviceCheck keys.
  name: apple-team-id
  source: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md
  type: platform-key
slug: triumph-authentication
source_filename: triumph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions\nsource: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md\nsummary:\n  types: [sdk-credentials]\n  notes: Triumph publishes no public REST API and no OAuth/apiKey HTTP schemes.\n    Access is through the TriumphSDK (Swift/Unity, iOS), configured with identifiers\n    issued in the Triumph developer dashboard plus Apple platform keys uploaded to\n    that dashboard.\nschemes:\n- name: gameId\n  type: sdk-configuration\n  description: Per-game identifier issued in the Triumph developer dashboard (game's\n    \"go live\" tab). Passed to Triumph.configure(id:) in Swift or set on\n    TriumphUnityNativeMethods.gameId in Unity. An empty gameId runs the SDK in\n    sandbox mode.\n  source: https://docs.triumpharcade.com/triumph-sdk/import-triumph.md\n- name: merchantId\n  type: sdk-configuration\n  description: Merchant identifier set alongside gameId\
  \ in the Unity\n    TriumphUnityNativeMethods integration.\n  source: https://docs.triumpharcade.com/triumph-sdk/import-triumph.md\n- name: apple-apns-key\n  type: platform-key\n  description: Apple Push Notification Service (APNs) key created in the Apple\n    Developer account and uploaded (with its Key ID) under Settings > Apple Keys in\n    the Triumph dashboard; used to notify players of tournament results.\n  source: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md\n- name: apple-devicecheck-key\n  type: platform-key\n  description: Apple DeviceCheck key created in the Apple Developer account and\n    uploaded to the Triumph dashboard; used to verify submitted scores come from a\n    real device.\n  source: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md\n- name: apple-team-id\n  type: platform-key\n  description: Apple Developer Team ID recorded in the Triumph dashboard alongside\n    the APNs and DeviceCheck keys.\n  source: https://docs.triumpharcade.com/triumph-sdk/keys-and-permissions.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triumph/refs/heads/main/authentication/triumph-authentication.yml
summary_line: sdk-credentials · 5 schemes
tags:
- Company
- Gaming
- Real-Money Gaming
- Tournaments
- Mobile Games
- SDK
- Payments
- Collectibles
---
