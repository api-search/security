---
api_key_in: []
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Signal Sciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Signal Sciences secures its APIs with token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Signal Sciences
provider_slug: signal-sciences
scheme_count: 2
schemes:
- description: 'A session token obtained by POSTing email + password credentials to /auth, which returns a token used to authenticate subsequent requests. Verified live: unauthenticated requests to /api/v0/* return HTTP 401 with a JSON {"message": ...} body.'
  name: sessionToken
  obtain: POST https://dashboard.signalsciences.net/api/v0/auth
  sources:
  - https://www.fastly.com/documentation/reference/api/ngwaf/
  type: token
- description: Personal API access tokens created from the user's account settings in the Next-Gen WAF console (dashboard.signalsciences.net), used to authenticate programmatic API requests without an interactive login.
  name: apiAccessToken
  sources:
  - https://www.fastly.com/documentation/signalsciences/using-our-api/
  type: token
slug: signal-sciences-authentication
source_filename: signal-sciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.fastly.com/documentation/reference/api/ngwaf/\ndocs: https://www.fastly.com/documentation/signalsciences/using-our-api/\nverified_probe: 'GET https://dashboard.signalsciences.net/api/v0/corps returns HTTP 401 {\"message\":\"Unauthorized: You must be logged in to call this API\"}'\nbase_url: https://dashboard.signalsciences.net/api/v0\nsummary:\n  types:\n  - token\n  token_transport: header\nschemes:\n- name: sessionToken\n  type: token\n  description: >-\n    A session token obtained by POSTing email + password credentials to\n    /auth, which returns a token used to authenticate subsequent requests.\n    Verified live: unauthenticated requests to /api/v0/* return HTTP 401 with a\n    JSON {\"message\": ...} body.\n  obtain: POST https://dashboard.signalsciences.net/api/v0/auth\n  sources:\n  - https://www.fastly.com/documentation/reference/api/ngwaf/\n- name: apiAccessToken\n  type: token\n  description: >-\n\
  \    Personal API access tokens created from the user's account settings in the\n    Next-Gen WAF console (dashboard.signalsciences.net), used to authenticate\n    programmatic API requests without an interactive login.\n  sources:\n  - https://www.fastly.com/documentation/signalsciences/using-our-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal-sciences/refs/heads/main/authentication/signal-sciences-authentication.yml
summary_line: token · 2 schemes
tags:
- Company
- Security
- Web Application Firewall
- WAF
- API Security
- RASP
- Application Security
- Bot Protection
---
