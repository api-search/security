---
api_key_in:
- header
api_specs:
- filename: rubicon-project-springserve-v1-openapi.yml
  format: yaml
  label: SpringServe UI API (v1)
  slug: rubicon-project-springserve-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/openapi/rubicon-project-springserve-v1-openapi.yml
- filename: rubicon-project-springserve-v0-openapi.yml
  format: yaml
  label: SpringServe UI API (v0)
  slug: rubicon-project-springserve-v0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/openapi/rubicon-project-springserve-v0-openapi.yml
- filename: rubicon-project-springserve-v1-openapi.yml
  format: yaml
  label: ClearLine API
  slug: rubicon-project-clearline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/openapi/rubicon-project-springserve-v1-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rubicon Project Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rubicon Project secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rubicon Project
provider_slug: rubicon-project
scheme_count: 2
schemes:
- description: 'SpringServe authorization token based authentication. The opaque token returned by POST /api/v1/auth (or /api/v0/auth) is sent bare in the Authorization header, with no scheme prefix — `Authorization: <token>`.'
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/rubicon-project-springserve-v0-openapi.yml
  - openapi/rubicon-project-springserve-v1-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'SpringServe bearer token authentication. The same POST /api/v1/auth response also carries a bearer_token, sent as `Authorization: Bearer <token>`.'
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/rubicon-project-springserve-v0-openapi.yml
  - openapi/rubicon-project-springserve-v1-openapi.yml
  type: http
slug: rubicon-project-authentication
source_filename: rubicon-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://springserve.atlassian.net/wiki/spaces/SSD/pages/1573617663/API+-+Getting+Started\ndocs:\n- https://springserve.atlassian.net/wiki/spaces/SSD/pages/1573617663/API+-+Getting+Started\n- https://springserve.atlassian.net/wiki/spaces/CLD/pages/3649929246/CL+-API+-+Getting+Started\n- https://console.springserve.com/api-docs\nderived_from:\n- openapi/rubicon-project-springserve-v1-openapi.yml\n- openapi/rubicon-project-springserve-v0-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  credential_issuance: self-service-within-account\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    SpringServe authorization token based authentication. The opaque token returned by\n    POST /api/v1/auth (or /api/v0/auth) is sent bare in the Authorization header, with no\n    scheme prefix\
  \ — `Authorization: <token>`.\n  sources:\n  - openapi/rubicon-project-springserve-v0-openapi.yml\n  - openapi/rubicon-project-springserve-v1-openapi.yml\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    SpringServe bearer token authentication. The same POST /api/v1/auth response also\n    carries a bearer_token, sent as `Authorization: Bearer <token>`.\n  sources:\n  - openapi/rubicon-project-springserve-v0-openapi.yml\n  - openapi/rubicon-project-springserve-v1-openapi.yml\ntoken_endpoint:\n  method: POST\n  paths:\n  - /api/v1/auth\n  - /api/v0/auth\n  operation_ids:\n  - auth_post\n  request_body:\n    email: API user email\n    password: API user password\n  response_fields:\n  - token\n  - bearer_token\n  note: >-\n    Credentials are a console user's own email and password — there is no separate client\n    ID / client secret. The docs recommend creating a dedicated API user with a plus-address\n    (name+api@example.com) via Settings\
  \ -> Users so API-originated changes are attributable\n    in the changelog.\ntoken_lifetime:\n  value: 2\n  unit: hours\n  source: https://springserve.atlassian.net/wiki/spaces/SSD/pages/1573617663/API+-+Getting+Started\n  note: 'Published verbatim: \"A token expires after two hours.\"'\nsession:\n  cookie_auth: true\n  note: >-\n    The hosted Swagger UI at /api-docs authenticates with the console session cookie by\n    default; token and bearer auth take precedence when supplied. Cookie/session auth is a\n    property of the docs host, not a documented integration path.\n  inspect_operations:\n  - session_get\n  - session_delete\naccount_context:\n  header: x-auth-context\n  description: >-\n    Every authenticated request runs in the context of the caller's currently active\n    account. Read it with GET /api/v1/accounts/current, change it with\n    POST /api/v1/accounts/{id}/set_current, or override it per-request with the\n    x-auth-context header. Multi-account integrations must\
  \ set this explicitly.\n  operations:\n  - accounts_current_get\n  - accounts_id_set_current_post\nimpersonation:\n  supported: true\n  operations:\n  - run_as_start_post\n  - run_as_stop_post\n  note: >-\n    A privileged \"run as\" surface exists (POST /api/v1/run_as/start, /stop) and returns 403\n    \"You are not authorized to access this page.\" when the caller lacks the grant.\ngaps:\n- No OAuth 2.0, OIDC or mTLS surface is published; there is no scoped third-party\n  authorization flow, so an integration holds full user-equivalent rights.\n- Password-grant style authentication means an integration stores a human user's console\n  password, and the docs offer no key rotation or revocation endpoint.\n- The 2-hour token lifetime is documented but no refresh endpoint is published; clients\n  must re-POST /auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/authentication/rubicon-project-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Advertising
- AdTech
- Programmatic Advertising
- Sell-Side Platform
- SSP
- Real-Time Bidding
- Connected TV
- Ad Serving
- Media
- OpenRTB
- Reporting
---
