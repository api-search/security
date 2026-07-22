---
api_key_in:
- sdk-config
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nexad Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Nexad secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Nexad
provider_slug: nexad
scheme_count: 2
schemes:
- credentials:
  - App ID
  - Publisher ID
  name: nexad-android-sdk
  product: Nexad Android Ads SDK
  provisioning: Credentials are issued after submitting the Nexad contact form; the team returns a unique App ID and Publisher ID passed to NexadSDK.initialize().
  source: https://docs.nex.ad/docs/android/getting-started
  type: apiKey
- detail: The Soku CLI authenticates via an OAuth device-login flow (`soku auth login`), issuing a bearer token stored locally (mode 0600). Direct calls to api.soku.ai/v1 and api.soku.ai/mcp return HTTP 401 without a token. Third-party provider credentials are injected server-side via `soku egress` rather than handled by the user.
  endpoint: https://api.soku.ai
  flow: deviceCode
  name: soku-nexstudio-api
  product: Soku (NexStudio) API
  source: https://soku.ai/cli/skill.md
  type: oauth2
slug: nexad-authentication
source_filename: nexad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource:\n  - https://docs.nex.ad/docs/android/getting-started\n  - https://soku.ai/cli/skill.md\nnotes: >-\n  Nexad has no published OpenAPI, so this profile is searched from provider docs\n  rather than derived. Two distinct products with distinct auth models.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [sdk-config]\n  oauth2_flows: [deviceCode]\nschemes:\n  - name: nexad-android-sdk\n    product: Nexad Android Ads SDK\n    type: apiKey\n    credentials:\n      - App ID\n      - Publisher ID\n    provisioning: >-\n      Credentials are issued after submitting the Nexad contact form; the team\n      returns a unique App ID and Publisher ID passed to NexadSDK.initialize().\n    source: https://docs.nex.ad/docs/android/getting-started\n  - name: soku-nexstudio-api\n    product: Soku (NexStudio) API\n    type: oauth2\n    flow: deviceCode\n    endpoint: https://api.soku.ai\n    detail: >-\n      The Soku CLI authenticates via\
  \ an OAuth device-login flow (`soku auth\n      login`), issuing a bearer token stored locally (mode 0600). Direct calls\n      to api.soku.ai/v1 and api.soku.ai/mcp return HTTP 401 without a token.\n      Third-party provider credentials are injected server-side via `soku egress`\n      rather than handled by the user.\n    source: https://soku.ai/cli/skill.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexad/refs/heads/main/authentication/nexad-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Advertising
- Marketing
- Marketing Automation
- Contextual Advertising
- Mobile SDK
- Agent
---
