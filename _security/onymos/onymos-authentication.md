---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Onymos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onymos secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onymos
provider_slug: onymos
scheme_count: 1
schemes:
- applies_to: Onymos DocEnhance REST API
  description: '"An Onymos API authorization token is required to perform any requests." Sent as a request header on both documented DocEnhance operations (POST /api/enhance and GET /api/enhance/results/{UUID}). The docs do not publish how the token is obtained, rotated, scoped or expired, and there is no self-service issuance page — the token arrives through the commercial onboarding.'
  in: header
  name: onymosIesAuthToken
  parameter_name: onymosIesAuthToken
  required: true
  sources:
  - https://onymos.com/api/onymos-docenhance-endpoints/
  type: apiKey
slug: onymos-authentication
source_filename: onymos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://onymos.com/api/onymos-docenhance-endpoints/ and\n  https://onymos.com/api/onymos-access-functions/\ndocs: https://onymos.com/api/onymos-docenhance-endpoints/\nnote: >-\n  Derived by reading the published reference pages, NOT from an OpenAPI document — Onymos publishes no\n  machine-readable contract, so there are no `securitySchemes` to aggregate and\n  0-working/derive-authentication.py had nothing to read. Two distinct and unrelated auth surfaces exist\n  and are kept separate below: (1) the service token that authorises calls to the Onymos DocEnhance REST\n  API, and (2) the end-user social sign-in that the Onymos Access component brokers on behalf of the\n  customer's app. (2) is NOT API authentication — Onymos never issues or holds those credentials; under\n  the No-Data Architecture the OAuth 2.0 exchange happens between the customer's app and Apple, Facebook\n  or Google.\nsummary:\n  types:\n  - apiKey\n\
  \  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2_scopes_documented: false\n  mutual_tls: false\n  openid_connect: false\nschemes:\n- name: onymosIesAuthToken\n  type: apiKey\n  in: header\n  parameter_name: onymosIesAuthToken\n  applies_to: Onymos DocEnhance REST API\n  required: true\n  description: >-\n    \"An Onymos API authorization token is required to perform any requests.\" Sent as a request header on\n    both documented DocEnhance operations (POST /api/enhance and GET /api/enhance/results/{UUID}). The\n    docs do not publish how the token is obtained, rotated, scoped or expired, and there is no\n    self-service issuance page — the token arrives through the commercial onboarding.\n  sources:\n  - https://onymos.com/api/onymos-docenhance-endpoints/\ndelegated_end_user_auth:\n- name: Onymos Access\n  protocol: OAuth 2.0 (delegated to third-party identity providers)\n  providers:\n  - apple\n  - facebook\n  - google\n  scope_parameter: >-\n    An optional `scope` option\
  \ is passed straight through to the provider — comma-separated for Facebook,\n    space-separated for Google. The scope strings are the providers' own, not an Onymos scope vocabulary,\n    which is why no scopes/ artifact is emitted for this provider.\n  operations:\n  - OnymosAccess.login\n  - OnymosAccess.logout\n  - OnymosAccess.getAuth\n  - OnymosAccess.listenForAuth\n  - OnymosAccess.stopListenForAuth\n  - OnymosAccess.signup\n  - OnymosAccess.resetPasswordRequest\n  - OnymosAccess.resetPassword\n  - OnymosAccess.getOtherUsersInfo\n  sources:\n  - https://onymos.com/api/onymos-access-functions/\n- name: Onymos Biometrics\n  protocol: device biometric (Face ID / Touch ID / Android biometric prompt)\n  operations:\n  - onymosBioAuth.isAvailable\n  - onymosBioAuth.authenticate\n  sources:\n  - https://onymos.com/api/onymos-biometrics-functions/\ngaps:\n- No published token-issuance, rotation or expiry policy for onymosIesAuthToken.\n- No OAuth 2.0 or OIDC surface of Onymos's own; no\
  \ /.well-known/openid-configuration (404).\n- No documented scope vocabulary, so scopes/ is deliberately not emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onymos/refs/heads/main/authentication/onymos-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Features as a Service
- SDK
- Application Development
- Mobile
- Document Processing
- Intelligent Document Processing
- OCR
- Healthcare
- Life Sciences
- Authentication
- Chat
- Push Notifications
- Geolocation
- Payments
- IoT
- No-Data Architecture
- Components
---
