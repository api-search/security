---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Contify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contify secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Contify
provider_slug: contify
scheme_count: 2
schemes:
- description: Application identifier issued to the API consumer. Sent on every request alongside APPSECRET; both headers are required.
  in: header
  name: APPID
  parameter_name: APPID
  sources:
  - https://www.contify.com/resources/blog/business-news-api-v4/
  type: apiKey
- description: Application secret paired with APPID. Sent as a plain request header over TLS; there is no published rotation, expiry or scope model.
  in: header
  name: APPSECRET
  parameter_name: APPSECRET
  sources:
  - https://www.contify.com/resources/blog/business-news-api-v4/
  type: apiKey
slug: contify-authentication
source_filename: contify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://www.contify.com/resources/blog/business-news-api-v4/\ndocs: https://developer.contify.com/api/login/?next=/api/\nnote: >-\n  Contify publishes no OpenAPI, so this profile was not derived from a spec. It was read\n  from the verbatim curl examples Contify itself publishes in its Business News API v4\n  announcement (screenshots at\n  https://www.contify.com/wp-content/uploads/2025/07/Request-Source-Curl-1024x128.png and\n  Ticker-Symbol-1024x99.png), and confirmed against the live API: an unauthenticated\n  GET https://api.contify.com/v4.1/updates returns HTTP 403\n  {\"detail\":\"Authentication credentials were not provided.\"}. The full reference sits\n  behind a login at developer.contify.com.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  scheme_count: 2\nschemes:\n  - name: APPID\n    type: apiKey\n    in: header\n    parameter_name: APPID\n    description: >-\n      Application\
  \ identifier issued to the API consumer. Sent on every request alongside\n      APPSECRET; both headers are required.\n    sources:\n      - https://www.contify.com/resources/blog/business-news-api-v4/\n  - name: APPSECRET\n    type: apiKey\n    in: header\n    parameter_name: APPSECRET\n    description: >-\n      Application secret paired with APPID. Sent as a plain request header over TLS;\n      there is no published rotation, expiry or scope model.\n    sources:\n      - https://www.contify.com/resources/blog/business-news-api-v4/\nobserved:\n  - url: https://api.contify.com/v4.1/updates\n    method: GET\n    status: 403\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    checked: '2026-09-05'\ngaps:\n  - No OAuth 2.0 or OpenID Connect surface is published or advertised.\n  - No scope or permission model is published; the key pair is all-or-nothing.\n  - No key-rotation, expiry, or revocation policy is published on a public page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contify/refs/heads/main/authentication/contify-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Competitive Intelligence
- Market Intelligence
- Business News
- News
- Artificial Intelligence
- Data
- Strategies
---
