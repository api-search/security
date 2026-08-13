---
api_key_in:
- header
api_specs:
- filename: optimyzee-openapi.yml
  format: yaml
  label: Optimyzee Application API
  slug: optimyzee-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimyzee/refs/heads/main/openapi/optimyzee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Optimyzee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optimyzee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Optimyzee
provider_slug: optimyzee
scheme_count: 1
schemes:
- description: Bearer token authorization
  in: header
  name: token
  note: Declared as an OpenAPI `apiKey` scheme rather than `http`/`bearer`, but the scheme's own description says "Bearer token authorization". Applied to 108 of 184 operations.
  parameter: authorization
  sources:
  - openapi/optimyzee-openapi.yml
  type: apiKey
slug: optimyzee-authentication
source_filename: optimyzee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/_original/optimyzee-openapi.json\ndocs: null\ndocs_note: >-\n  Optimyzee publishes no authentication documentation - there is no developer portal, API reference or\n  help center to upgrade this profile from. Everything below is read out of the harvested contract or\n  observed on a live anonymous request to https://api.optimyzee.com.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  user_issuable_api_key: false\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: Bearer token authorization\n  sources:\n  - openapi/optimyzee-openapi.yml\n  note: >-\n    Declared as an OpenAPI `apiKey` scheme rather than `http`/`bearer`, but the scheme's own\n    description says \"Bearer token authorization\". Applied to 108 of 184 operations.\ncoverage:\n  operations_total: 184\n  operations_with_security: 108\n \
  \ operations_without_security: 76\n  root_level_security_default: null\n  note: >-\n    The document declares no root-level `security`, so the 76 operations with no `security` block are\n    unconstrained by the contract. Some are legitimately anonymous (sign-in, signup, password reset),\n    but 23 of them are on the internal /operations/* back-office surface, including\n    POST /operations/user/{userId}/impersonate. The contract does not say whether those are genuinely\n    open or simply under-declared.\ntoken_lifecycle:\n  mint:\n  - {operation: appAuthGatewayEmail, http: 'POST /app/auth/gateway/email'}\n  - {operation: appAuthGatewayEmailSignup, http: 'POST /app/auth/gateway/emailSignup'}\n  - {operation: appAuthGatewayGoogle, http: 'POST /app/auth/gateway/google'}\n  - {operation: appAuthGatewayGoogleSignup, http: 'POST /app/auth/gateway/googleSignup'}\n  - {operation: appAuthGatewayFacebook, http: 'POST /app/auth/gateway/facebook'}\n  - {operation: appAuthGatewayFacebookSignup,\
  \ http: 'POST /app/auth/gateway/facebookSignup'}\n  refresh:\n  - {operation: appAuthGatewayRefresh, http: 'POST /app/auth/gateway/refresh'}\n  revoke:\n  - {operation: appAuthGatewayRevoke, http: 'POST /app/auth/gateway/revoke'}\n  schema: AppAuthGatewayTokenSchema\n  staff_equivalent:\n  - {operation: operationsAuthGateway, http: 'POST /operations/auth/gateway'}\naccount_security_surface:\n  two_factor:\n  - 'POST /app/auth/tfa/issue'\n  - 'POST /app/auth/tfa/enable'\n  - 'POST /app/auth/tfa/disable'\n  trusted_devices:\n  - 'GET,POST /app/auth/trustedDevice'\n  - 'POST /app/auth/trustedDevice/current'\n  - 'GET,DELETE /app/auth/trustedDevice/{trustedDeviceId}'\n  email_verification:\n  - 'POST /app/auth/email'\n  - 'POST /app/auth/email/verify'\n  - 'POST /app/auth/email/resend'\n  password:\n  - 'POST /app/auth/password/sendResetLink'\n  - 'POST /app/auth/password/reset'\n  note: >-\n    TOTP two-factor and trusted-device management are first-class in the contract - a stronger account\n\
  \    security posture than the absence of any published security documentation would suggest.\ndelegated_authorization:\n  note: >-\n    Optimyzee is an OAuth *client*, not an OAuth server. It consumes Google Ads, Meta and Yelp\n    authorizations on the user's behalf via /app/linking/g, /app/linking/meta and /app/yelp/connection\n    (authorization-code exchange with `code` + `redirectUri`), but exposes no authorization server,\n    no scopes and no consent surface of its own. /.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration both returned 404 on optimyzee.com and api.optimyzee.com.\ntransport:\n  https_only: true\n  observed_tls: TLSv1.3\n  hsts_on_api_host: false\n  cors_allow_origin: '*'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimyzee/refs/heads/main/authentication/optimyzee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Advertising
- Google Ads
- PPC
- Marketing
- Automation
- Artificial Intelligence
- SaaS
- Campaign Management
- Search Advertising
- Yelp Ads
- Meta Ads
- Keyword Research
- Reporting
---
