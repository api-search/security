---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Workerbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workerbase secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Workerbase
provider_slug: workerbase
scheme_count: 2
schemes:
- in: header
  name: accessToken
  parameter: accesstoken
  sources:
  - npm @workerbase/sdk (Config.accessToken = WB_ACCESS_TOKEN; header `accesstoken`)
  - npm node-red-contrib-workerbase (credential node access token)
  type: apiKey
- description: Username/password login that yields the access token used by API calls.
  endpoint: POST {instanceUrl}/usermanagement/auth/login
  name: instanceLogin
  scheme: login-endpoint
  sources:
  - npm node-red-contrib-workerbase (workerbase-credentials.js)
  type: http
slug: workerbase-authentication
source_filename: workerbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: npm @workerbase/sdk 1.0.6 + node-red-contrib-workerbase 1.1.0 (first-party code)\ndocs: https://workerbase.zendesk.com/hc/en-us (login required)\nnotes: >-\n  No public OpenAPI exists, so this profile is taken from Workerbase's own published client\n  code. The platform API is per-tenant (the customer's Workerbase instance URL). The JavaScript\n  SDK (which runs inside Workerbase Functions) authenticates with an access token supplied via\n  the WB_ACCESS_TOKEN environment variable and sent as an `accesstoken` request header. The\n  Node-RED nodes authenticate the same way, obtaining tokens via a username/password login\n  endpoint. No OAuth 2.0 / OIDC surface was found (no /.well-known/openid-configuration or\n  oauth-authorization-server documents on the primary host).\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_name: accesstoken\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter:\
  \ accesstoken\n  sources:\n  - npm @workerbase/sdk (Config.accessToken = WB_ACCESS_TOKEN; header `accesstoken`)\n  - npm node-red-contrib-workerbase (credential node access token)\n- name: instanceLogin\n  type: http\n  scheme: login-endpoint\n  description: Username/password login that yields the access token used by API calls.\n  endpoint: POST {instanceUrl}/usermanagement/auth/login\n  sources:\n  - npm node-red-contrib-workerbase (workerbase-credentials.js)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workerbase/refs/heads/main/authentication/workerbase-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Manufacturing
- Connected Worker
- Frontline Operations
- Digital Work Instructions
- Quality Management
- Maintenance
- Industrial IoT
---
