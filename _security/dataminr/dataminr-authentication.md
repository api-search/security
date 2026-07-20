---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dataminr Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Dataminr secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Dataminr
provider_slug: dataminr
scheme_count: 1
schemes:
- description: Client-credentials grant. The integration exchanges a client_id and client_secret at the token endpoint for a short-lived access token (dmaToken) plus a refresh token, then presents the token on each request.
  flow: clientCredentials
  name: PulseOAuth2
  refresh_field: refreshToken
  request_header: 'Authorization: Dmauth <dmaToken>'
  sources:
  - https://developer.dataminr.com
  - live probe gateway.dataminr.com
  token_field: dmaToken
  token_url: https://gateway.dataminr.com/auth/2/token
  type: oauth2
slug: dataminr-authentication
source_filename: dataminr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.dataminr.com\nnotes: >-\n  No public OpenAPI is published. Auth model captured from Dataminr's developer\n  portal and confirmed by live probes of the Pulse API gateway\n  (gateway.dataminr.com): the token endpoint /auth/2/token exists (HTTP 405 on\n  GET, 500 on empty POST) and protected resources such as /api/3/alerts and\n  /account/2/get_lists return HTTP 401 without a bearer token.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  token_delivery: bearer\nschemes:\n- name: PulseOAuth2\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Client-credentials grant. The integration exchanges a client_id and\n    client_secret at the token endpoint for a short-lived access token\n    (dmaToken) plus a refresh token, then presents the token on each request.\n  token_url: https://gateway.dataminr.com/auth/2/token\n  token_field: dmaToken\n  refresh_field: refreshToken\n\
  \  request_header: 'Authorization: Dmauth <dmaToken>'\n  sources:\n  - https://developer.dataminr.com\n  - live probe gateway.dataminr.com\nhosts:\n  api_gateway: https://gateway.dataminr.com\nverified_endpoints:\n- path: /auth/2/token\n  method: POST\n  observed_status: 405-on-GET / 500-on-empty-POST\n  note: token endpoint present, requires POST body\n- path: /api/3/alerts\n  method: GET\n  observed_status: 401\n  note: bearer token required\n- path: /account/2/get_lists\n  method: GET\n  observed_status: 401\n  note: bearer token required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataminr/refs/heads/main/authentication/dataminr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Analytics
- Threat Intelligence
- Risk
- Real-Time
- Security
- Artificial Intelligence
- Alerting
---
