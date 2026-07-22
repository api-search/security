---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mattermark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mattermark secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mattermark
provider_slug: mattermark
scheme_count: 1
schemes:
- applies_to:
  - https://api.mattermark.com/
  - https://eapi.mattermark.com/
  description: 'Mattermark authenticates REST (https://api.mattermark.com/) and GraphQL (https://eapi.mattermark.com/) requests with an API key passed as an HTTP Bearer token in the Authorization header: "Authorization: Bearer <your api key>". Keys are issued from the API Settings section of a Mattermark account. There is no OAuth 2.0 / OpenID Connect surface and no scope model.'
  format: Bearer <api key>
  header: Authorization
  key_provisioning: Mattermark account -> API Settings
  name: bearerAuth
  scheme: bearer
  type: http
slug: mattermark-authentication
source_filename: mattermark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.mattermark.com/docs/rest-requests-authentication\ndocs: https://developer.mattermark.com/docs\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Mattermark authenticates REST (https://api.mattermark.com/) and GraphQL\n    (https://eapi.mattermark.com/) requests with an API key passed as an HTTP\n    Bearer token in the Authorization header: \"Authorization: Bearer <your api\n    key>\". Keys are issued from the API Settings section of a Mattermark\n    account. There is no OAuth 2.0 / OpenID Connect surface and no scope model.\n  header: Authorization\n  format: 'Bearer <api key>'\n  key_provisioning: Mattermark account -> API Settings\n  applies_to:\n  - https://api.mattermark.com/\n  - https://eapi.mattermark.com/\nnotes:\n- No published OpenAPI/Swagger security scheme document was\
  \ available (docs are\n  hosted on a ReadMe hub); this profile was searched from the developer docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/authentication/mattermark-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Business Intelligence
- Company Data
- Investors
- Funding
- Sales Intelligence
- Market Research
---
