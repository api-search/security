---
api_key_in: []
api_specs:
- filename: rtbhouse-advertisers-api-openapi.yml
  format: yaml
  label: RTB House Advertisers API
  slug: rtbhouse-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-advertisers-api-openapi.yml
- filename: rtbhouse-dev-api-openapi.yml
  format: yaml
  label: RTB House Dev API
  slug: rtbhouse-dev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-dev-api-openapi.yml
- filename: rtbhouse-statistics-api-openapi.yml
  format: yaml
  label: RTB House Statistics API
  slug: rtbhouse-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-statistics-api-openapi.yml
- filename: rtbhouse-tokens-api-openapi.yml
  format: yaml
  label: RTB House Tokens API
  slug: rtbhouse-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-tokens-api-openapi.yml
- filename: rtbhouse-user-api-openapi.yml
  format: yaml
  label: RTB House User API
  slug: rtbhouse-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-user-api-openapi.yml
auth_types:
- http
description: The RTB House Client Panel API v5 authenticates with HTTP Authorization headers only. The OpenAPI declares two schemes (http basic, http bearer); the first-party SDK documents a third accepted style — an `Authorization` header carrying `Token <api-token>` — which the spec does not mention. There is no OAuth, no OIDC, no API key parameter and no mTLS. Every path except GET /healthcheck requires a credential.
kind: authentication
layout: security
method: searched
name: Rtbhouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: RTB House secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RTB House
provider_slug: rtbhouse
scheme_count: 3
schemes:
- credential: API token minted in the Clients Panel
  header: 'Authorization: Bearer <api-token>'
  name: bearerAuth
  preferred: true
  scheme: bearer
  sources:
  - openapi/rtbhouse-advertisers-api-openapi.yml
  - openapi/rtbhouse-dev-api-openapi.yml
  - openapi/rtbhouse-statistics-api-openapi.yml
  - openapi/rtbhouse-tokens-api-openapi.yml
  - openapi/rtbhouse-user-api-openapi.yml
  type: http
- credential: Clients Panel username and password
  header: 'Authorization: Basic <base64(username:password)>'
  name: basicAuth
  note: The API returns a WWW-Authenticate header of `Basic realm="application"` on a 401, observed live 2026-08-13.
  scheme: basic
  sources:
  - openapi/rtbhouse-advertisers-api-openapi.yml
  - openapi/rtbhouse-dev-api-openapi.yml
  - openapi/rtbhouse-statistics-api-openapi.yml
  - openapi/rtbhouse-tokens-api-openapi.yml
  - openapi/rtbhouse-user-api-openapi.yml
  type: http
- credential: fixed API token
  header: 'Authorization: Token <api-token>'
  header_note: An Authorization header carrying the literal scheme name Token.
  in_spec: false
  name: tokenScheme
  note: Accepted by the API but absent from the published securitySchemes — a contract gap, not a second credential type.
  scheme: token
  sources:
  - https://github.com/rtbhouse-apps/rtbhouse-python-sdk (BasicTokenAuth / _HttpxBasicTokenAuth)
  type: http
slug: rtbhouse-authentication
source_filename: rtbhouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/rtbhouse-advertisers-api-openapi.yml, openapi/rtbhouse-dev-api-openapi.yml,\n  openapi/rtbhouse-statistics-api-openapi.yml, openapi/rtbhouse-tokens-api-openapi.yml,\n  openapi/rtbhouse-user-api-openapi.yml; upgraded from https://github.com/rtbhouse-apps/rtbhouse-python-sdk\n  (README.rst \"Authentication methods\", rtbhouse_sdk/client.py) and live probes of\n  https://api.panel.rtbhouse.com/v5/ on 2026-08-13\ndocs: https://api.panel.rtbhouse.com/api/docs\ncredential_issuance: https://panel.rtbhouse.com/user/api-tokens\ndescription: >-\n  The RTB House Client Panel API v5 authenticates with HTTP Authorization\n  headers only. The OpenAPI declares two schemes (http basic, http bearer); the\n  first-party SDK documents a third accepted style — an `Authorization` header carrying\n  `Token <api-token>` — which the spec does not mention. There is no OAuth, no OIDC, no\n  API key parameter and no mTLS. Every path except GET\
  \ /healthcheck requires a\n  credential.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  - token (undocumented in the spec; accepted per the first-party SDK)\n  api_key_in: []\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <api-token>'\n  credential: API token minted in the Clients Panel\n  preferred: true\n  sources:\n  - openapi/rtbhouse-advertisers-api-openapi.yml\n  - openapi/rtbhouse-dev-api-openapi.yml\n  - openapi/rtbhouse-statistics-api-openapi.yml\n  - openapi/rtbhouse-tokens-api-openapi.yml\n  - openapi/rtbhouse-user-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  header: 'Authorization: Basic <base64(username:password)>'\n  credential: Clients Panel username and password\n  note: >-\n    The API returns a WWW-Authenticate header of `Basic realm=\"application\"` on a 401,\n    observed live 2026-08-13.\n  sources:\n \
  \ - openapi/rtbhouse-advertisers-api-openapi.yml\n  - openapi/rtbhouse-dev-api-openapi.yml\n  - openapi/rtbhouse-statistics-api-openapi.yml\n  - openapi/rtbhouse-tokens-api-openapi.yml\n  - openapi/rtbhouse-user-api-openapi.yml\n- name: tokenScheme\n  type: http\n  scheme: token\n  header: 'Authorization: Token <api-token>'\n  header_note: An Authorization header carrying the literal scheme name Token.\n  credential: fixed API token\n  in_spec: false\n  sources:\n  - https://github.com/rtbhouse-apps/rtbhouse-python-sdk (BasicTokenAuth /\n    _HttpxBasicTokenAuth)\n  note: Accepted by the API but absent from the published securitySchemes — a contract\n    gap, not a second credential type.\ntoken_lifecycle:\n  expiring: true\n  expiry_on_inactivity: true\n  expiry_note: RTB House API tokens have a limited lifetime AND expire if they are not\n    actively used. An integration that calls infrequently loses its credential.\n  rotation_operation: POST /tokens/current/rotate\n  rotation_response:\
  \ '{status: ok, data: {token, expiresAt}}'\n  rotation_window: The token becomes eligible for rotation before expiry; the SDK checks\n    eligibility on every request and rotates within that window.\n  read_current_token: not possible — no read operation exists; the rotation response is\n    the only time a new token is disclosed\n  tooling:\n  - ApiTokenManager / AsyncApiTokenManager (automatic rotation, pluggable storage)\n  - ApiTokenAuth (static token, no rotation)\n  - python -m rtbhouse_sdk.api_tokens init-json | keep-alive-json (see ../cli/rtbhouse-cli.yml)\nauthorization:\n  model: coarse per-user permissions\n  signal: GET /user/info returns `permissions` (string array), plus `isClientUser` and\n    `isDemoUser` flags\n  scopes: none — there is no OAuth scope surface, so no scopes/ artifact is emitted\n  note: Access is otherwise scoped by which advertiser hashes GET /advertisers returns\n    for the authenticated user.\nunauthenticated_operations:\n- GET /healthcheck\ntransport:\n\
  \  https_required: true\n  hsts: max-age=31536000 on api.panel.rtbhouse.com\n  cors_allowed_origin: https://panel.rtbhouse.com\n  cors_note: Cross-origin browser access is limited to the first-party panel; the API is\n    not callable from a third-party web origin.\nfailure_mode:\n  status: 401\n  app_code: INVALID_CREDENTIALS\n  body: '{\"message\": \"Unauthorized\", \"status\": \"error\", \"httpCode\": 401, \"appCode\":\n    \"INVALID_CREDENTIALS\"}'\n  observed: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/authentication/rtbhouse-authentication.yml
summary_line: http · 3 schemes
tags:
- Advertising
- Retargeting
- Programmatic
- DSP
- Deep Learning
- RTB
- Performance Marketing
---
