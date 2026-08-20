---
api_key_in: []
api_specs:
- filename: kardinal-aro-openapi-original.yml
  format: yaml
  label: Kardinal ARO API
  slug: aro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kardinal/refs/heads/main/openapi/kardinal-aro-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kardinal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kardinal secures its APIs with http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kardinal
provider_slug: kardinal
scheme_count: 5
schemes:
- bearerFormat: JWT
  lifetime: 1 hour
  name: access_token
  purpose: The working credential. Sent on every business operation (plans, resources, orders, solutions).
  scheme: bearer
  sources:
  - openapi/kardinal-aro-openapi-original.yml
  type: http
- bearerFormat: JWT
  lifetime: 30 days (per the provider-published agent skill)
  name: refresh_token
  purpose: Exchanged at POST /login/refresh for a new access_token without re-sending the password.
  scheme: bearer
  sources:
  - openapi/kardinal-aro-openapi-original.yml
  type: http
- bearerFormat: JWT
  name: otp_token
  purpose: Interim token issued by POST /login when MFA is configured; redeemed at POST /login/otp.
  scheme: bearer
  sources:
  - openapi/kardinal-aro-openapi-original.yml
  type: http
- bearerFormat: JWT
  name: password_token
  purpose: Issued by the password-reset request flow; redeemed at POST /auth/password/reset.
  scheme: bearer
  sources:
  - openapi/kardinal-aro-openapi-original.yml
  type: http
- bearerFormat: JWT
  name: gdpr_token
  purpose: Declared in the spec's securitySchemes for GDPR-scoped access.
  scheme: bearer
  sources:
  - openapi/kardinal-aro-openapi-original.yml
  type: http
slug: kardinal-authentication
source_filename: kardinal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/kardinal-aro-openapi-original.yml\ndocs: https://developers.kardinal.ai/guides/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - JWT\n  oauth2_flows: []\n  api_key_in: []\n  model: >-\n    Username/password exchanged for a short-lived JWT access token, sent as\n    `Authorization: Bearer <access_token>`. There is no long-lived, dashboard-issued\n    API key. Five distinct bearer token classes are declared in the spec, each gating\n    a different stage of the login / MFA / recovery lifecycle.\nschemes:\n- name: access_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  purpose: The working credential. Sent on every business operation (plans, resources, orders, solutions).\n  lifetime: 1 hour\n  sources: [openapi/kardinal-aro-openapi-original.yml]\n- name: refresh_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  purpose: Exchanged at POST /login/refresh\
  \ for a new access_token without re-sending the password.\n  lifetime: 30 days (per the provider-published agent skill)\n  sources: [openapi/kardinal-aro-openapi-original.yml]\n- name: otp_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  purpose: Interim token issued by POST /login when MFA is configured; redeemed at POST /login/otp.\n  sources: [openapi/kardinal-aro-openapi-original.yml]\n- name: password_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  purpose: Issued by the password-reset request flow; redeemed at POST /auth/password/reset.\n  sources: [openapi/kardinal-aro-openapi-original.yml]\n- name: gdpr_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  purpose: Declared in the spec's securitySchemes for GDPR-scoped access.\n  sources: [openapi/kardinal-aro-openapi-original.yml]\ntoken_verification:\n  public_key_endpoint: GET /public_key\n  unauthenticated: true\n  formats: [JWK, PEM]\n  observed:\n    url: https://app.kardinal.ai/api/v2/public_key\n\
  \    http_status: 200\n    algorithm: ES384\n    key_type: EC P-384\n    note: >-\n      Probed anonymously on 2026-08-17 and returned a real JWK. Tokens are\n      asymmetrically signed, so integrators can verify them offline.\nflows:\n- name: password login\n  steps: [POST /login]\n  operation_ids: [postLogin]\n  returns: [access_token, refresh_token]\n- name: MFA / OTP login\n  steps: [POST /login, POST /login/otp]\n  operation_ids: [postLogin, postLoginOTP]\n  resend: {operation_id: requestNewLoginOTPCode, path: POST /login/resendOTP, rate_limited: true, status_on_exhaustion: 429}\n- name: token refresh\n  steps: [POST /login/refresh]\n  operation_ids: [postLoginRefresh]\n- name: Azure SSO\n  steps: [POST /login/sso/azure]\n  operation_ids: [postLoginWithAzureSSO]\n- name: Google SSO\n  steps: [POST /login/sso/google]\n  operation_ids: [postLoginWithGoogleSSO]\n- name: password reset\n  steps: [POST /auth/password/requestToken, POST /auth/password/validateToken, POST /auth/password/reset]\n\
  \  operation_ids: [postRequestPasswordToken, validatePasswordToken, resetPassword]\n- name: MFA configuration\n  steps: [GET /auth/mfa/config, POST /auth/mfa/request, POST /auth/mfa/validate, PUT /auth/mfa/preferredType, POST /auth/mfa/disable, PUT /auth/mfa/regenerateBackupCodes]\n  operation_ids: [getActorMFAConfig, requestMFAConfigUpdate, validateMFAConfigUpdate, putMFAConfigPreferredType, disableMFAConfig, regenerateMFABackupCodes]\n  resend: {operation_id: requestNewMFAOTPCode, path: POST /auth/mfa/resendOTP, rate_limited: true, status_on_exhaustion: 429}\nprovisioning:\n  self_serve: false\n  model: invitation\n  note: >-\n    Per https://developers.kardinal.ai/getting-started/first-api-call, access is\n    provisioned by invitation — a user is invited to set a password on a per-customer\n    environment host, and there is no self-serve sign-up flow. Credentials are\n    requested from an Account Executive or api@kardinal.ai.\n  environments: per-customer, https://<env>.kardinal.ai,\
  \ sandbox and production fully separate\nrevocation:\n  self_service: false\n  note: >-\n    The docs state there is no documented self-service revocation endpoint; a\n    suspected compromise is handled by contacting api@kardinal.ai or the Account\n    Executive.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kardinal/refs/heads/main/authentication/kardinal-authentication.yml
summary_line: http · 5 schemes
tags:
- Company
- Software-as-a-Service
- Route Optimization
- Vehicle Routing
- Last Mile Delivery
- Logistics
- Supply Chain
- Transportation
- Fleet Management
- Optimization
---
