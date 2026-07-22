---
api_key_in:
- sdk-initialization
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Synervoz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synervoz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synervoz
provider_slug: synervoz
scheme_count: 1
schemes:
- description: Switchboard SDK is initialized with an appID and appSecret pair issued per application. Developers sign up for a free account to obtain the appID and appSecret values, which are supplied to the SDK at initialization time (SwitchboardSDK.initialize(appID, appSecret)) across all platform bindings (iOS/Swift, Android/Kotlin, JavaScript, React Native, C++).
  name: AppCredentials
  obtain: Sign up for a free account, then retrieve appID/appSecret from the downloads/onboarding page.
  parameters:
  - appID
  - appSecret
  sources:
  - https://docs.switchboard.audio/downloads/
  type: apiKey
slug: synervoz-authentication
source_filename: synervoz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.switchboard.audio/downloads/\ndocs: https://docs.switchboard.audio/\nsummary:\n  types: [apiKey]\n  api_key_in: [sdk-initialization]\n  model: app-credential\nschemes:\n  - name: AppCredentials\n    type: apiKey\n    description: >-\n      Switchboard SDK is initialized with an appID and appSecret pair issued per\n      application. Developers sign up for a free account to obtain the appID and\n      appSecret values, which are supplied to the SDK at initialization time\n      (SwitchboardSDK.initialize(appID, appSecret)) across all platform bindings\n      (iOS/Swift, Android/Kotlin, JavaScript, React Native, C++).\n    parameters:\n      - appID\n      - appSecret\n    obtain: Sign up for a free account, then retrieve appID/appSecret from the downloads/onboarding page.\n    sources:\n      - https://docs.switchboard.audio/downloads/\nnotes: >-\n  This is a client-SDK credential model, not a hosted REST OAuth\
  \ surface — there\n  is no documented OAuth2/OIDC flow or token endpoint. Credentials gate SDK\n  initialization; some audio-graph nodes are cloud-integrated and use the same\n  app credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synervoz/refs/heads/main/authentication/synervoz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Audio
- SDK
- Voice
- Real-Time Communication
- Speech
- Developer Tools
- Cross-Platform
---
