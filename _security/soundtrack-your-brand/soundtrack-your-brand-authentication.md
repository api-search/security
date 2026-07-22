---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Soundtrack Your Brand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soundtrack Your Brand secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Soundtrack Your Brand
provider_slug: soundtrack-your-brand
scheme_count: 2
schemes:
- description: 'Provisioned API client token sent as `Authorization: Basic <token>`. Request credentials via the API docs page. Compromised tokens are blocked.'
  header: 'Authorization: Basic <token>'
  name: apiTokenBasic
  provisioning: https://api.soundtrackyourbrand.com/v2/docs
  scheme: basic
  sources:
  - https://api.soundtrackyourbrand.com/v2/docs
  type: http
- description: 'Access token obtained from the loginUser mutation (email + password) or the OTP flow (generateOTP / loginOTP), sent as `Authorization: Bearer <token>`. Not recommended for production API clients (the underlying user can be rate limited or suspended). Returns HTTP 401 when expired.'
  name: userBearer
  obtained_via:
  - loginUser
  - generateOTP
  - loginOTP
  - loginDevice
  refresh_via: refreshLogin
  scheme: bearer
  sources:
  - https://api.soundtrackyourbrand.com/v2/docs
  subscriptions: token supplied as a query parameter on the subscription connection
  type: http
slug: soundtrack-your-brand-authentication
source_filename: soundtrack-your-brand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.soundtrackyourbrand.com/v2/docs\ndocs: https://api.soundtrackyourbrand.com/v2/docs\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Soundtrack GraphQL API is a single endpoint that authenticates over HTTP\n    Authorization headers. API clients use HTTP Basic with a provisioned API\n    token. Applications acting on behalf of a Soundtrack user instead obtain a\n    Bearer access token via the loginUser mutation and refresh it with\n    refreshLogin. There is no OAuth2 authorization-code flow and no scope surface.\nschemes:\n  - name: apiTokenBasic\n    type: http\n    scheme: basic\n    description: >-\n      Provisioned API client token sent as `Authorization: Basic <token>`.\n      Request credentials via the API docs page. Compromised tokens are blocked.\n    header: 'Authorization: Basic <token>'\n    provisioning: https://api.soundtrackyourbrand.com/v2/docs\n\
  \    sources: [https://api.soundtrackyourbrand.com/v2/docs]\n  - name: userBearer\n    type: http\n    scheme: bearer\n    description: >-\n      Access token obtained from the loginUser mutation (email + password) or the\n      OTP flow (generateOTP / loginOTP), sent as `Authorization: Bearer <token>`.\n      Not recommended for production API clients (the underlying user can be rate\n      limited or suspended). Returns HTTP 401 when expired.\n    obtained_via: [loginUser, generateOTP, loginOTP, loginDevice]\n    refresh_via: refreshLogin\n    subscriptions: token supplied as a query parameter on the subscription connection\n    sources: [https://api.soundtrackyourbrand.com/v2/docs]\nmutations:\n  - loginUser        # email/password -> { token, refreshToken }\n  - refreshLogin     # refreshToken   -> { token, refreshToken }\n  - generateOTP\n  - loginOTP\n  - loginDevice\n  - generateStreamingUrl\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundtrack-your-brand/refs/heads/main/authentication/soundtrack-your-brand-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Music
- Music Streaming
- Background Music
- GraphQL
- Retail
- Hospitality
- Audio
- API
---
