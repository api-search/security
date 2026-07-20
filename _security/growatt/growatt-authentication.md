---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Growatt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Growatt secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Growatt
provider_slug: growatt
scheme_count: 1
schemes:
- description: Account-scoped Open API V1 token, issued from openapi.growatt.com and sent on every request.
  in: header
  name: growattToken
  parameter_name: token
  sources:
  - https://www.showdoc.com.cn/262556420217021/0
  type: apiKey
slug: growatt-authentication
source_filename: growatt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.showdoc.com.cn/262556420217021/0\ndocs: https://www.showdoc.com.cn/262556420217021/0\nnotes: >-\n  Growatt Open API V1 uses a static API token issued to the account. The token is\n  sent on every request in a `token` HTTP header. Tokens are obtained by an account\n  holder from the Growatt Open API console (openapi.growatt.com). The legacy\n  ShinePhone API instead used username/password (MD5) session login; V1 token auth\n  is the officially supported, recommended mechanism.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: growattToken\n  type: apiKey\n  in: header\n  parameter_name: token\n  description: Account-scoped Open API V1 token, issued from openapi.growatt.com and\n    sent on every request.\n  sources:\n  - https://www.showdoc.com.cn/262556420217021/0\nlegacy:\n- name: shinephoneLogin\n  type: session\n  scheme: username/password (MD5) login, cookie session\n\
  \  status: deprecated-in-favor-of-v1-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growatt/refs/heads/main/authentication/growatt-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer Technology
- Solar
- Energy
- Photovoltaic
- Inverters
- Energy Storage
- IoT
- Monitoring
---
