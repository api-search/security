---
api_key_in:
- header
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Hiya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hiya secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hiya
provider_slug: hiya
scheme_count: 2
schemes:
- applies_to:
  - Hiya Connect API
  - Hiya Protect API
  - Hiya AI Voice Platform API
  description: 'App ID and App Secret are concatenated as "AppID:AppSecret", base64-encoded, and sent as "Authorization: Basic <credentials>". The App ID carries an environment prefix (e.g. PROD_SampleApp) to distinguish production from test. The encoded string must have no leading/trailing spaces or line breaks.'
  format: Basic base64(AppID:AppSecret)
  header: Authorization
  in: header
  name: BasicAuth
  scheme: basic
  source: https://developer.hiya.com/docs/getting-started/authentication
  type: http
- applies_to:
  - Hiya Audio Intelligence API
  description: Audio Intelligence authenticates with bearer tokens. A token is obtained by signing in with credentials (credentials-sign-in) or via managed API keys (keys-create / keys-list). The AI Voice Platform also exposes a get-hiya-auth-token operation for issuing auth tokens.
  format: Bearer <token>
  header: Authorization
  in: header
  name: BearerAuth
  scheme: bearer
  source: https://developer.hiya.com/docs/audio-intel/endpoints/credentials-sign-in
  type: http
slug: hiya-authentication
source_filename: hiya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.hiya.com/docs/getting-started/authentication\ndocs: https://developer.hiya.com/docs/getting-started/authentication\nsummary:\n  types: [http-basic, http-bearer]\n  api_key_in: [header]\n  notes: >-\n    Most Hiya REST APIs (Connect, Protect, AI Voice Platform) use HTTP Basic\n    authentication over HTTPS with an App ID and App Secret. The Audio\n    Intelligence API uses bearer tokens obtained via a credentials sign-in\n    endpoint. Credentials are issued as separate Test and Production key pairs\n    via the self-service Console or by contacting Hiya.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  format: 'Basic base64(AppID:AppSecret)'\n  description: >-\n    App ID and App Secret are concatenated as \"AppID:AppSecret\", base64-encoded,\n    and sent as \"Authorization: Basic <credentials>\". The App ID carries an\n    environment prefix (e.g. PROD_SampleApp)\
  \ to distinguish production from test.\n    The encoded string must have no leading/trailing spaces or line breaks.\n  applies_to: [Hiya Connect API, Hiya Protect API, Hiya AI Voice Platform API]\n  source: https://developer.hiya.com/docs/getting-started/authentication\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n  description: >-\n    Audio Intelligence authenticates with bearer tokens. A token is obtained by\n    signing in with credentials (credentials-sign-in) or via managed API keys\n    (keys-create / keys-list). The AI Voice Platform also exposes a\n    get-hiya-auth-token operation for issuing auth tokens.\n  applies_to: [Hiya Audio Intelligence API]\n  source: https://developer.hiya.com/docs/audio-intel/endpoints/credentials-sign-in\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiya/refs/heads/main/authentication/hiya-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Voice Security
- Caller ID
- Branded Calling
- Spam Protection
- Scam Protection
- Deepfake Detection
- Voice Authentication
- Telecommunications
- Call Analytics
---
