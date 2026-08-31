---
api_key_in: []
auth_types:
- appCredentials
description: ''
kind: authentication
layout: security
method: searched
name: Voxer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voxer secures its APIs with appCredentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voxer
provider_slug: voxer
scheme_count: 1
schemes:
- credentials:
  - appId
  - appSecret
  - userId
  description: Per-client appId + appSecret pair provisioned by Voxer; required to initialize the SDK and to log a user (unique user id) into the Voxer network.
  name: voxerSdkAppCredentials
  self_service: false
  sources:
  - https://github.com/Voxer/voxer.io.api.docs/blob/master/android/v1.0/README.md
  type: appCredentials
slug: voxer-authentication
source_filename: voxer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/Voxer/voxer.io.api.docs/blob/master/android/v1.0/README.md\ndocs: https://github.com/Voxer/voxer.io.api.docs\nsummary:\n  types: [appCredentials]\n  notes: >-\n    Voxer publishes no public REST API, so there are no OpenAPI securitySchemes\n    to derive. The documented developer surface is the Voxer SDK (Android v1.0,\n    iOS v0.4), whose authentication model is app credentials: every SDK client\n    is provisioned a unique appId + appSecret, which initialize the SDK, and\n    end users then log into the Voxer network with a unique user id via\n    Voxer.getInstance(application).login(username, appId, appSecret). SDK\n    credentials are issued through a gated early-access program, not\n    self-service.\nschemes:\n- name: voxerSdkAppCredentials\n  type: appCredentials\n  description: >-\n    Per-client appId + appSecret pair provisioned by Voxer; required to\n    initialize the SDK and to log a user (unique\
  \ user id) into the Voxer\n    network.\n  credentials: [appId, appSecret, userId]\n  self_service: false\n  sources:\n  - https://github.com/Voxer/voxer.io.api.docs/blob/master/android/v1.0/README.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxer/refs/heads/main/authentication/voxer-authentication.yml
summary_line: appCredentials · 1 scheme
tags:
- Company
- Communications
- Push-To-Talk
- Walkie-Talkie
- Voice
- Messaging
- Mobile
- SDK
---
