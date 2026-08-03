---
api_key_in:
- header
api_specs:
- filename: rentberry-openapi.yml
  format: yaml
  label: Rentberry API
  slug: rentberry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentberry/refs/heads/main/openapi/rentberry-openapi.yml
auth_types:
- token
description: ''
kind: authentication
layout: security
method: derived
name: Rentberry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rentberry secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rentberry
provider_slug: rentberry
scheme_count: 1
schemes:
- applied_to_operations: 122
  defined_in_spec: false
  in: header
  name: XAuthToken
  note: Referenced by name only. The header name `X-Auth-Token` is inferred from the scheme name and is NOT published by Rentberry; it must be confirmed with the provider before use.
  parameter_name: X-Auth-Token
  parameter_name_confidence: low
  sources:
  - openapi/rentberry-openapi.yml
  type: apiKey
slug: rentberry-authentication
source_filename: rentberry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/rentberry-openapi.yml\ndocs: https://api.rentberry.com/docs\nsummary:\n  types:\n  - token\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The Rentberry OpenAPI 3.0.0 applies a security requirement named `XAuthToken` to 122 of its 220\n    operations, but `components.securitySchemes` is ABSENT from the document — the scheme is referenced\n    and never defined. This is a spec defect captured in overlays/rentberry-openapi-overlay.yaml, not an\n    API Evangelist assumption: the token flow below is reconstructed from the auth operations that the\n    spec DOES describe, plus live probes of api.rentberry.com.\nschemes:\n- name: XAuthToken\n  type: apiKey\n  in: header\n  parameter_name: X-Auth-Token\n  parameter_name_confidence: low\n  defined_in_spec: false\n  applied_to_operations: 122\n  sources:\n  - openapi/rentberry-openapi.yml\n  note: >-\n    Referenced by name only. The header name `X-Auth-Token`\
  \ is inferred from the scheme name and is NOT\n    published by Rentberry; it must be confirmed with the provider before use.\ntoken_acquisition:\n- operationId: post_api_v1_auth_token\n  method: POST\n  path: /v{version}/auth/token\n  summary: Authenticate user and get token\n  request:\n    required:\n    - username\n    - plainPassword\n    optional:\n    - oauthConnectId\n    - oauthProvider\n    - isRaiUser\n  response:\n    '200': '{\"auth_token\": \"<string>\"}'\n    '400': Validation failed\n    '401': Authentication failed\n    '1005': User blocked or not verified\n- operationId: get_api_v2_auth_session\n  method: GET\n  path: /v{version}/auth\n  summary: Get current user session information (returns auth boolean + notification counters)\n- operationId: post_api_v1_auth_email_otp_request\n  method: POST\n  path: /v{version}/auth/email-otp/request\n  summary: Request an email one-time passcode\n- operationId: post_api_v1_auth_email_otp_verify\n  method: POST\n  path: /v{version}/auth/email-otp/verify\n\
  \  summary: Verify an email one-time passcode\nsocial_login:\n  note: >-\n    The `OAuth` tag covers END-USER social login into Rentberry accounts (Google, Apple) — it is NOT a\n    third-party OAuth 2.0 authorization server for API consumers. No /.well-known/openid-configuration or\n    /.well-known/oauth-authorization-server is served on rentberry.com or api.rentberry.com (both 404 on\n    2026-08-02), and the spec declares no oauth2 security scheme, so no scopes/ artifact is emitted.\n  providers:\n  - google\n  - apple\n  operations:\n  - get_api_v1_oauth_init\n  - get_api_v1_oauth_authorize\n  - post_api_v4_google_one_tap\n  - get_api_v1_oauth_authorize_by_short_lived_access_token\n  - post_api_v4_oauth_apple_callback\n  - delete_api_v1_oauth_authorize_disconnect_user\ndevice_identity:\n  header: X-Device-Token\n  operations:\n  - get_api_v1_device_list\n  - put_api_v1_device_update\n  - post_api_v1_device_register\n  - delete_api_v1_device_delete\n  - put_api_v1_device_link_user\n\
  \  note: A separate device-scoped header used by the Devices operations for push registration.\nroles:\n  note: >-\n    Operation descriptions carry role requirements in prose, e.g. \"Requires ROLE_USER\". These are Symfony\n    security roles, not OAuth scopes, and are not machine-readable in the spec.\n  observed:\n  - ROLE_USER\nx-evidence:\n- fetched: '2026-08-02'\n  url: https://api.rentberry.com/v2/auth\n  http_status: 403\n  body: '{\"body\":null,\"error\":{\"code\":403,\"message\":\"Oops, error occurred\",\"description\":\"Not enough rights\"}}'\n  note: Unauthenticated request to a token-protected operation.\n- fetched: '2026-08-02'\n  url: https://api.rentberry.com/.well-known/openid-configuration\n  http_status: 404\n- fetched: '2026-08-02'\n  url: https://api.rentberry.com/.well-known/oauth-authorization-server\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentberry/refs/heads/main/authentication/rentberry-authentication.yml
summary_line: token · 1 scheme
tags:
- real-estate
- proptech
- rentals
- rental-marketplace
- property-management
- tenant-screening
- e-signature
- payments
- listings
- search
- geocoding
- marketplace
---
