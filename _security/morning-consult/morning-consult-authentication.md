---
api_key_in: []
api_specs:
- filename: morning-consult-openapi-original.yml
  format: yaml
  label: Morning Consult API
  slug: morning-consult-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/openapi/morning-consult-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Morning Consult Authentication
name_suffix: Authentication
oauth_flows: []
overview: Morning Consult secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Morning Consult
provider_slug: morning-consult
scheme_count: 3
schemes:
- description: Username and password credentials for initial authentication.
  name: Basic
  scheme: basic
  sources:
  - openapi/morning-consult-openapi-original.yml
  type: http
  used_by:
  - postAuthToken
- bearerFormat: JWT
  default: true
  description: JWT Bearer header authentication for performing regular requests.
  name: JWT
  scheme: bearer
  sources:
  - openapi/morning-consult-openapi-original.yml
  type: http
  used_by: all operations except postAuthToken
- description: Refresh Token bearer header authentication for renewing tokens.
  name: RefreshToken
  note: Declared in components.securitySchemes and listed as the alternate security requirement on POST /auth/token. Missed by the mechanical derive pass, which collapses http/bearer schemes; recovered from the spec and the docs.
  scheme: bearer
  sources:
  - openapi/morning-consult-openapi-original.yml
  type: http
  used_by:
  - postAuthToken
slug: morning-consult-authentication
source_filename: morning-consult-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/morning-consult-openapi-original.yml\ndocs: https://api.morningconsult.com/docs/#authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  model: >-\n    Two-step. HTTP Basic credentials (a Morning Consult Intelligence username and\n    password issued by the customer's Account Executive) are exchanged at\n    POST /auth/token for a short-lived JWT plus a refresh token. Every other operation\n    is authenticated with the JWT as an Authorization: Bearer header. There is no OAuth\n    2.0 authorization server, no OIDC discovery document, no API key, and no scope\n    surface — entitlement is carried in the JWT's claims and enforced per subscription.\ndefault_security:\n- JWT\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: Username and password credentials for initial authentication.\n  used_by:\n  - postAuthToken\n  sources:\n\
  \  - openapi/morning-consult-openapi-original.yml\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer header authentication for performing regular requests.\n  default: true\n  used_by: all operations except postAuthToken\n  sources:\n  - openapi/morning-consult-openapi-original.yml\n- name: RefreshToken\n  type: http\n  scheme: bearer\n  description: Refresh Token bearer header authentication for renewing tokens.\n  used_by:\n  - postAuthToken\n  note: >-\n    Declared in components.securitySchemes and listed as the alternate security\n    requirement on POST /auth/token. Missed by the mechanical derive pass, which\n    collapses http/bearer schemes; recovered from the spec and the docs.\n  sources:\n  - openapi/morning-consult-openapi-original.yml\ntoken:\n  endpoint: POST /auth/token\n  operation_id: postAuthToken\n  request_auth: Basic (initial) or RefreshToken bearer (renewal)\n  response_fields:\n    id_token: The JWT to send in the Authorization\
  \ header on all other requests.\n    refresh_token: Exchange for a new token pair before expiry.\n    expires_in: Seconds until the JWT expires (3600 in the published example/default).\n    token_type: Bearer\n  expiry_seconds: 3600\n  rotation: >-\n    Exchange refresh_token at POST /auth/token before expires_in elapses. Credential\n    exchange is limited to one request per second and 20 per minute per username;\n    refresh-token requests are limited to 30 per minute.\n  errors:\n  - invalid credentials\n  - invalid or expired refresh token\nprovisioning:\n  self_service: false\n  process: >-\n    Credentials are issued by the customer's Morning Consult Account Executive. API\n    access is included with a Morning Consult Intelligence subscription at no additional\n    cost but must be enabled for the account.\n  sso_note: >-\n    Accounts that authenticate to MCI with SSO must request a separate API password from\n    their Account Executive, because SSO cannot mint a JWT at POST /auth/token.\n\
  \  signup: https://morningconsult.com/book-a-demo\nscopes:\n  present: false\n  note: No OAuth scopes. Authorization is claim-based — a 403 \"missing necessary claims\"\n    is returned when the JWT lacks an entitlement (e.g. bulk / Data Bridge access).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/authentication/morning-consult-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Market Research
- Survey Data
- Consumer Intelligence
- Brand Tracking
- Decision Intelligence
- Public Opinion
- Analytics
- Data
- Artificial Intelligence
---
