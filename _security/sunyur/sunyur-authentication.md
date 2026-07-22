---
api_key_in:
- query
auth_types:
- accessToken
description: ''
kind: authentication
layout: security
method: searched
name: Sunyur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunyur secures its APIs with accessToken across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sunyur
provider_slug: sunyur
scheme_count: 1
schemes:
- description: Access token required on open-platform API calls; passed as the accessToken request parameter. Provisioned through the Sunyur open platform developer console (login required).
  in: query
  name: accessToken
  parameter: accessToken
  sources:
  - live-observed https://open.sunyur.com/api
  type: apiKey
slug: sunyur-authentication
source_filename: sunyur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://open.sunyur.com/api (live-observed API auth challenge)\nsummary:\n  types: [accessToken]\n  api_key_in: [query]\n  oauth2_flows: []\n  notes: >-\n    Sunyur exposes an enterprise procurement open platform (\"聚贤阁\") at\n    https://open.sunyur.com. The public API base at https://open.sunyur.com/api\n    rejects unauthenticated calls with resultCode 20111\n    (\"accessToken 参数不允许为空\" / \"the accessToken parameter must not be empty\"),\n    confirming a token-based auth model where callers present an accessToken.\n    The developer console API under /front/ is separately session/login gated\n    (code 50003, \"请登录后访问\" / \"login required\"). Full credential-provisioning\n    flow (appKey/appSecret exchange) is documented behind the login-gated\n    developer docs at https://open.sunyur.com/front/#/docs and could not be\n    captured verbatim.\nschemes:\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: accessToken\n\
  \  sources: [live-observed https://open.sunyur.com/api]\n  description: >-\n    Access token required on open-platform API calls; passed as the accessToken\n    request parameter. Provisioned through the Sunyur open platform developer\n    console (login required).\ndocs: https://open.sunyur.com/front/#/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunyur/refs/heads/main/authentication/sunyur-authentication.yml
summary_line: accessToken · 1 scheme
tags:
- Company
- Procurement
- SRM
- E-Procurement
- Supplier Management
- Digital Procurement
- Enterprise Software
- SaaS
- B2B
- China
- AI
---
