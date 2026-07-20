---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: August Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: August Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: August Health
provider_slug: august-health
scheme_count: 1
schemes:
- bearer_format: JWT
  description: 'JWT id token passed as `Authorization: Bearer {idToken}`. Tokens are scoped to a specific API user and can be used across all endpoints for organizations the user has access to.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.augusthealth.com/docs/authentication-tokens.md
  type: http
slug: august-health-authentication
source_filename: august-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.augusthealth.com/docs/authentication-tokens.md\ndocs: https://developer.augusthealth.com/docs/authentication-tokens.md\nsummary:\n  types: [http]\n  scheme: bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\n  model: >-\n    Token-based bearer authentication. Clients obtain a short-lived JWT id token\n    from the token endpoint using API user credentials, then pass it as\n    `Authorization: Bearer {idToken}`. Access is governed by named permissions\n    granted to the API user (e.g. BILLING_PAYMENTS_CREATE), not OAuth scopes.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    JWT id token passed as `Authorization: Bearer {idToken}`. Tokens are scoped to\n    a specific API user and can be used across all endpoints for organizations the\n    user has access to.\n  sources: [https://developer.augusthealth.com/docs/authentication-tokens.md]\n\
  token_endpoint:\n  operation: createTokenV1\n  path: /v1/token\n  method: POST\n  flows:\n  - name: credentials\n    request: '{ \"credentials\": { \"username\": \"...\", \"password\": \"...\" } }'\n  - name: refresh\n    request: '{ \"refreshCredentials\": { \"idToken\": \"...\", \"refreshToken\": \"...\" } }'\n  response_fields:\n  - idToken\n  - refreshToken\n  - tokenType (Bearer)\n  - expiresIn (seconds until id token expiry)\n  token_lifetimes:\n    id_token: short-lived; refresh at 80-90% of expiresIn\n    refresh_token: 24 hours\npermissions_model:\n  style: named-permissions\n  note: >-\n    Endpoints require specific named permissions on the API user. Documented\n    example: `BILLING_PAYMENTS_CREATE` is required for the Record deposit\n    operation. There is no OAuth2 authorization-server / scope flow; this is a\n    permission-gated bearer-JWT model, so no scopes/ artifact is emitted.\n  observed_permissions:\n  - name: BILLING_PAYMENTS_CREATE\n    required_by: recordDepositV1\n\
  \    source: https://developer.augusthealth.com/reference/recorddepositv1.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/august-health/refs/heads/main/authentication/august-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- EHR
- Senior Living
- Eldercare
- Electronic Health Records
- eMAR
- Billing
- Webhooks
- API
---
