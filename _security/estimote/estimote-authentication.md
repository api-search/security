---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Estimote Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Estimote secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Estimote
provider_slug: estimote
scheme_count: 2
schemes:
- description: HTTP Basic authentication where the username is your Estimote App ID and the password is your App Token. Both are issued per-app in the Apps section of Estimote Cloud and act as login/password for programmatic access to your account's devices and attachments.
  name: appIdTokenBasic
  scheme: basic
  source: https://forums.estimote.com/t/what-are-app-id-and-app-token-and-what-do-i-need-them-for/7066
  type: http
- flows:
  - authorizationUrl: https://cloud.estimote.com/v1/oauth2/authorize
    flow: authorizationCode
    scopes: {}
    tokenUrl: https://cloud.estimote.com/v1/oauth2/access_token
  name: oauth2AuthorizationCode
  registration: Client ID and client secret are issued manually by Estimote (private beta) on request.
  source: https://developer.estimote.com/cloud/oauth/
  status: private-beta
  token_usage: 'Authorization: Bearer ACCESS_TOKEN'
  type: oauth2
slug: estimote-authentication
source_filename: estimote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.estimote.com/cloud/oauth/\ndocs: https://developer.estimote.com/cloud/oauth/\nsummary:\n  types: [http, oauth2]\n  api_key_in: []\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Estimote Cloud API is authenticated primarily with an App ID and App Token pair\n    (created in the Apps section of Estimote Cloud) sent as HTTP Basic credentials\n    (curl -u APP_ID:APP_TOKEN). App-level OAuth 2.0 (authorization code) is available in\n    private beta for third-party apps acting on behalf of other Estimote accounts; the\n    resulting bearer access token is sent in the Authorization header.\nschemes:\n  - name: appIdTokenBasic\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication where the username is your Estimote App ID and the\n      password is your App Token. Both are issued per-app in the Apps section of Estimote\n      Cloud and\
  \ act as login/password for programmatic access to your account's devices\n      and attachments.\n    source: https://forums.estimote.com/t/what-are-app-id-and-app-token-and-what-do-i-need-them-for/7066\n  - name: oauth2AuthorizationCode\n    type: oauth2\n    status: private-beta\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://cloud.estimote.com/v1/oauth2/authorize\n        tokenUrl: https://cloud.estimote.com/v1/oauth2/access_token\n        scopes: {}\n    token_usage: 'Authorization: Bearer ACCESS_TOKEN'\n    registration: >-\n      Client ID and client secret are issued manually by Estimote (private beta) on request.\n    source: https://developer.estimote.com/cloud/oauth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estimote/refs/heads/main/authentication/estimote-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Location
- Proximity
- Beacons
- Bluetooth
- IoT
- Indoor Location
- UWB
- Asset Tracking
- Developer Tools
---
