---
api_key_in: []
auth_types:
- tracking-id
- device-login
description: ''
kind: authentication
layout: security
method: searched
name: Liv Authentication
name_suffix: Authentication
oauth_flows: []
overview: LIV secures its APIs with tracking-id and device-login across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LIV
provider_slug: liv
scheme_count: 2
schemes:
- description: UUID v4 Tracking ID configured at SDK init (LckCore.Initialize / Unreal project settings). Missing/invalid IDs surface as CoreError.MissingTrackingId (Unity) or error code 1 InvalidTrackingId (Unreal).
  issued_by: https://dashboard.liv.tv
  kind: developer-identifier
  name: tracking-id
- description: End-user login for streaming/subscription. LckCore.StartLoginAttemptAsync() returns a login code the user confirms in LIV Hub; the app polls LckCore.CheckLoginCompletedAsync() until the attempt completes, then queries IsUserSubscribed() / HasUserConfiguredStreaming().
  kind: user-authentication
  name: liv-hub-login
  operations:
  - StartLoginAttemptAsync
  - CheckLoginCompletedAsync
  - IsUserSubscribed
  - HasUserConfiguredStreaming
slug: liv-authentication
source_filename: liv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.liv.tv/api-reference/unity/classes/core/LckCore.md\nnotes: >-\n  LIV Camera Kit is a client SDK, not a REST API; there is no OpenAPI securityScheme\n  to derive. Authentication is handled inside the SDK via a Tracking ID plus a LIV\n  Hub device-login flow. The app authenticates the end user (viewer) for streaming\n  and subscription features; the developer identifies their integration with a\n  Tracking ID (UUID v4) issued from the LIV Developer Dashboard.\nsummary:\n  types: [tracking-id, device-login]\n  developer_credential: Tracking ID (UUID v4) issued in the LIV Developer Dashboard\n  user_auth: LIV Hub login-code (device authorization style) polling flow\nschemes:\n- name: tracking-id\n  kind: developer-identifier\n  description: >-\n    UUID v4 Tracking ID configured at SDK init (LckCore.Initialize / Unreal project\n    settings). Missing/invalid IDs surface as CoreError.MissingTrackingId (Unity) or\n \
  \   error code 1 InvalidTrackingId (Unreal).\n  issued_by: https://dashboard.liv.tv\n- name: liv-hub-login\n  kind: user-authentication\n  description: >-\n    End-user login for streaming/subscription. LckCore.StartLoginAttemptAsync()\n    returns a login code the user confirms in LIV Hub; the app polls\n    LckCore.CheckLoginCompletedAsync() until the attempt completes, then queries\n    IsUserSubscribed() / HasUserConfiguredStreaming().\n  operations:\n  - StartLoginAttemptAsync\n  - CheckLoginCompletedAsync\n  - IsUserSubscribed\n  - HasUserConfiguredStreaming\ndocs: https://docs.liv.tv/api-reference/unity/classes/core/LckCore.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liv/refs/heads/main/authentication/liv-authentication.yml
summary_line: tracking-id/device-login · 2 schemes
tags:
- Company
- XR
- Virtual Reality
- Mixed Reality
- Video Capture
- Live Streaming
- Game Engine SDK
- Unity
- Unreal Engine
- Meta Quest
---
