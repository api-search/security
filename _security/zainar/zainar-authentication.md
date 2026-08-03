---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zainar Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZaiNar secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ZaiNar
provider_slug: zainar
scheme_count: 3
schemes:
- description: Opaque API token issued by the platform's own token endpoint and sent verbatim in the Authorization request header on every subsequent call.
  in: header
  name: zainarToken
  parameter: Authorization
  scheme: bearer
  sources:
  - https://github.com/zainar/locate-latency-measurement-script/blob/main/rest_client.py
  type: http
- description: Alternate machine-to-machine credential (SERVICE_KEY) supported by the client in place of an interactive token; format is not published.
  in: header
  name: zainarServiceKey
  parameter: Authorization
  scheme: other
  sources:
  - https://github.com/zainar/locate-latency-measurement-script/blob/main/rest_client.py
  type: http
- description: JWT session cookie issued by the ZaiNar Positioning System (ZLP) web console at zps.zainartech.com; used to authenticate the Socket.IO real-time location stream. Browser-session credential, not a documented API credential.
  in: cookie
  name: zpsSessionCookie
  parameter: __session
  sources:
  - https://github.com/zainar/locate-latency-measurement-script/blob/main/README.md
  type: apiKey
slug: zainar-authentication
source_filename: zainar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: https://github.com/zainar/locate-latency-measurement-script\nsource_files:\n- rest_client.py\n- env_config.example.json\n- README.md\nnote: 'ZaiNar publishes no OpenAPI definition and no public authentication documentation.\n  This profile is DERIVED from ZaiNar''s own open-source client (github.com/zainar),\n  which implements the real authentication flow against the production Wi-Fi location\n  cloud. Nothing here is invented; every field traces to a line in that first-party\n  repository. Access is credential-gated — ZaiNar issues usernames and passwords to\n  customers; there is no public sign-up.'\nsummary:\n  types: [http]\n  api_key_in: []\n  oauth2_flows: []\n  public_signup: false\n  self_service: false\nschemes:\n- name: zainarToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: 'Opaque API token issued by the platform''s own token endpoint and\n    sent verbatim in the Authorization\
  \ request header on every subsequent call.'\n  sources: ['https://github.com/zainar/locate-latency-measurement-script/blob/main/rest_client.py']\n- name: zainarServiceKey\n  type: http\n  scheme: other\n  in: header\n  parameter: Authorization\n  description: 'Alternate machine-to-machine credential (SERVICE_KEY) supported by\n    the client in place of an interactive token; format is not published.'\n  sources: ['https://github.com/zainar/locate-latency-measurement-script/blob/main/rest_client.py']\n- name: zpsSessionCookie\n  type: apiKey\n  in: cookie\n  parameter: __session\n  description: 'JWT session cookie issued by the ZaiNar Positioning System (ZLP) web\n    console at zps.zainartech.com; used to authenticate the Socket.IO real-time\n    location stream. Browser-session credential, not a documented API credential.'\n  sources: ['https://github.com/zainar/locate-latency-measurement-script/blob/main/README.md']\ntoken_flow:\n  grant: password\n  endpoint: POST {baseURL}/authenticate\n\
  \  request_body: {username: string, password: string}\n  response_body: {token: string}\n  unauthenticated: true\n  presentation: 'Authorization: <token>'\n  refresh_interval_seconds: 1200\n  refresh_note: 'The first-party client refreshes the token every 20 minutes (TOKEN_REFRESH\n    = 20 * 60) and caches it on disk between runs; the server-side expiry is not published.'\nenvironments:\n- name: prod-us\n  base_url: https://api.wifi-prd-us.zainar.net/pipeline/r/api/v2/client\n  production: true\n- name: prod-apac\n  base_url: https://api.wifi-prd-jpn.zainar.net/pipeline/r/api/v2/client\n  production: true\n- name: int\n  base_url: https://api.wifi-int.zainar.net/pipeline/r/api/v2/client\n  production: false\n- name: dev\n  base_url: https://api.wifi-dev.zainar.net/pipeline/r/api/v2/client\n  production: false\ngaps:\n- No public authentication documentation page.\n- No OAuth 2.0 or OpenID Connect surface; no /.well-known/openid-configuration or\n  /.well-known/oauth-authorization-server\
  \ on any host (see well-known/zainar-well-known.yml).\n- No scopes or permissions model published — scopes/ is intentionally absent.\n- Token lifetime and revocation semantics are not published.\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://raw.githubusercontent.com/zainar/locate-latency-measurement-script/main/rest_client.py\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zainar/refs/heads/main/authentication/zainar-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Location
- Positioning
- Navigation
- Timing
- Wireless
- Real-Time Location
- Asset Tracking
- IoT
- Physical AI
---
