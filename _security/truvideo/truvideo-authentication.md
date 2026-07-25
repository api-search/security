---
api_key_in: []
api_specs:
- filename: truvideo-authentication-api-openapi.yml
  format: yaml
  label: TruVideo Authentication API
  slug: truvideo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-authentication-api-openapi.yml
- filename: truvideo-chat-api-openapi.yml
  format: yaml
  label: TruVideo Chat API
  slug: truvideo-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-chat-api-openapi.yml
- filename: truvideo-customers-api-openapi.yml
  format: yaml
  label: TruVideo Customers API
  slug: truvideo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-customers-api-openapi.yml
- filename: truvideo-dealers-api-openapi.yml
  format: yaml
  label: TruVideo Dealers API
  slug: truvideo-dealers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-dealers-api-openapi.yml
- filename: truvideo-files-api-openapi.yml
  format: yaml
  label: TruVideo Files API
  slug: truvideo-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-files-api-openapi.yml
- filename: truvideo-messages-api-openapi.yml
  format: yaml
  label: TruVideo Messages API
  slug: truvideo-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-messages-api-openapi.yml
- filename: truvideo-repair-orders-api-openapi.yml
  format: yaml
  label: TruVideo Repair Orders API
  slug: truvideo-repair-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-repair-orders-api-openapi.yml
- filename: truvideo-reports-api-openapi.yml
  format: yaml
  label: TruVideo Reports API
  slug: truvideo-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-reports-api-openapi.yml
- filename: truvideo-support-api-openapi.yml
  format: yaml
  label: TruVideo Support API
  slug: truvideo-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-support-api-openapi.yml
- filename: truvideo-users-api-openapi.yml
  format: yaml
  label: TruVideo Users API
  slug: truvideo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-users-api-openapi.yml
- filename: truvideo-videos-api-openapi.yml
  format: yaml
  label: TruVideo Videos API
  slug: truvideo-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/openapi/truvideo-videos-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Truvideo Authentication
name_suffix: Authentication
oauth_flows: []
overview: TruVideo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TruVideo
provider_slug: truvideo
scheme_count: 1
schemes:
- bearer_format: JWT
  description: Bearer JWT required on all endpoints except the login endpoint. Token is obtained from POST /api/v2/authentication/login and invalidated via POST /api/v2/authentication/logout.
  location: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  type: http
slug: truvideo-authentication
source_filename: truvideo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  TruVideo API documentation (github.com/Truvideo/Documentation:\n  authentication.md, README.md) and openapi/truvideo-openapi.yml.\ndocs: https://github.com/Truvideo/Documentation/blob/master/authentication.md\nsummary: >-\n  TruVideo's REST API uses JWT bearer-token authentication. Clients exchange\n  email + password at the login endpoint for a JWT, then send it in the\n  Authorization header (Bearer <token>) on every subsequent request. Sandbox\n  access requires a TruVideo Sandbox account; integration is gated\n  (devmgr+git@truvideo.com).\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    location: header\n    parameter: Authorization\n    description: >-\n      Bearer JWT required on all endpoints except the login endpoint. Token is\n      obtained from POST /api/v2/authentication/login and invalidated via\n      POST /api/v2/authentication/logout.\ntoken_endpoint:\n\
  \  operation: authLogin\n  method: POST\n  path: /api/v2/authentication/login\n  request: { email: string, password: string }\n  response: { token: JWT }\nlogout_endpoint:\n  operation: authLogout\n  method: POST\n  path: /api/v2/authentication/logout\nchat_token:\n  note: >-\n    The in-app chat surface issues a separate per-device custom token via\n    GET /chat/authentication/{deviceId}.\nnotes:\n  - All account-scoped requests carry an {accountId} (dealer id) path parameter.\n  - No OAuth 2.0 / OpenID Connect flow is documented; auth is a first-party JWT login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truvideo/refs/heads/main/authentication/truvideo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Commerce
- Video
- Messaging
- Automotive
- Communications
- SDK
- Video Intelligence
---
