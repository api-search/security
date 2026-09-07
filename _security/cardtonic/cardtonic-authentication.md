---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cardtonic-openapi.yml
  format: yaml
  label: Cardtonic Business API
  slug: business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardtonic/refs/heads/main/openapi/cardtonic-openapi.yml
auth_types: []
description: 'The Cardtonic Business API publishes no OpenAPI securitySchemes (components.securitySchemes is empty and every operation carries security: []), so this profile is read from the documented operations themselves rather than derived from the spec. Access is a two-stage model: a business user signs up and logs in to obtain a session token, then mints a long-lived API key through POST /users/generate-key. Every documented request additionally requires an X-Tonic-Env environment-selector header.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cardtonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cardtonic declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cardtonic
provider_slug: cardtonic
scheme_count: 3
schemes:
- description: Environment selector, required on all 14 documented operations. The only value published in Cardtonic's own examples is "development". This is a routing header, not a credential.
  evidence: parameters[] on every operation in openapi/cardtonic-openapi.yml
  id: tonic-env-header
  in: header
  name: X-Tonic-Env
  required: true
  source: https://docs.cardtonic.com/sign-up-business-user-11716510e0.md
  type: apiKey
- description: POST /auth/login/business exchanges an email + password for a session token. Cardtonic does not document the header the token is presented in; the login response body carries a "token" field. Email verification is enforced before login succeeds - an unverified account returns 403 "you're yet to verify your email".
  evidence: responses of loginBusiness / verifyEmail in openapi/cardtonic-openapi.yml
  gap: 'The presentation header (Authorization: Bearer vs a custom header) is not published. An integrator cannot construct an authenticated call from the documentation alone.'
  id: business-session-token
  operations:
  - loginBusiness
  - verifyEmail
  - resendEmailVerification
  - forgotPassword
  - resetPassword
  scheme: bearer
  source: https://docs.cardtonic.com/login-business-11716513e0.md
  type: http
- description: POST /users/generate-key issues a private API key; GET /users/show-api-key returns the current one. Cardtonic's own response example shows the key carries a "PRIV_" prefix followed by 64 hex characters. The transport header for the key is not documented.
  evidence: data.apiKey in the 200 response of generateApiKey
  gap: No securityScheme, no header name, no rotation or revocation operation is published.
  id: cardtonic-api-key
  key_prefix: PRIV_
  operations:
  - generateApiKey
  - fetchApiKey
  source: https://docs.cardtonic.com/generate-api-key-11716518e0.md
  type: apiKey
slug: cardtonic-authentication
source_filename: cardtonic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Cardtonic\nproviderId: cardtonic\ngenerated: '2026-09-05'\nmethod: searched\nsource: https://docs.cardtonic.com - the Auth and User operation pages of Cardtonic's published API documentation\nmodified: '2026-09-05'\ndescription: >-\n  The Cardtonic Business API publishes no OpenAPI securitySchemes (components.securitySchemes is\n  empty and every operation carries security: []), so this profile is read from the documented\n  operations themselves rather than derived from the spec. Access is a two-stage model: a business\n  user signs up and logs in to obtain a session token, then mints a long-lived API key through\n  POST /users/generate-key. Every documented request additionally requires an X-Tonic-Env\n  environment-selector header.\ndocs:\n  - https://docs.cardtonic.com\n  - https://cardtonic.com/developer\nschemes:\n  - id: tonic-env-header\n    type: apiKey\n    in: header\n    name: X-Tonic-Env\n\
  \    required: true\n    description: >-\n      Environment selector, required on all 14 documented operations. The only value published in\n      Cardtonic's own examples is \"development\". This is a routing header, not a credential.\n    evidence: 'parameters[] on every operation in openapi/cardtonic-openapi.yml'\n    source: https://docs.cardtonic.com/sign-up-business-user-11716510e0.md\n  - id: business-session-token\n    type: http\n    scheme: bearer\n    description: >-\n      POST /auth/login/business exchanges an email + password for a session token. Cardtonic does\n      not document the header the token is presented in; the login response body carries a \"token\"\n      field. Email verification is enforced before login succeeds - an unverified account returns\n      403 \"you're yet to verify your email\".\n    operations:\n      - loginBusiness\n      - verifyEmail\n      - resendEmailVerification\n      - forgotPassword\n      - resetPassword\n    evidence: 'responses of\
  \ loginBusiness / verifyEmail in openapi/cardtonic-openapi.yml'\n    source: https://docs.cardtonic.com/login-business-11716513e0.md\n    gap: >-\n      The presentation header (Authorization: Bearer vs a custom header) is not published. An\n      integrator cannot construct an authenticated call from the documentation alone.\n  - id: cardtonic-api-key\n    type: apiKey\n    description: >-\n      POST /users/generate-key issues a private API key; GET /users/show-api-key returns the\n      current one. Cardtonic's own response example shows the key carries a \"PRIV_\" prefix followed\n      by 64 hex characters. The transport header for the key is not documented.\n    operations:\n      - generateApiKey\n      - fetchApiKey\n    key_prefix: PRIV_\n    evidence: 'data.apiKey in the 200 response of generateApiKey'\n    source: https://docs.cardtonic.com/generate-api-key-11716518e0.md\n    gap: >-\n      No securityScheme, no header name, no rotation or revocation operation is published.\n\
  mfa:\n  supported: true\n  description: >-\n    Account-level two-factor authentication is togglable through POST /users/enable-2fa and\n    POST /users/disable-2fa. Neither the factor type (TOTP, SMS, email) nor the challenge/verify\n    step is documented.\n  operations:\n    - enable2fa\n    - disable2fa\nidentity_verification:\n  description: >-\n    Business accounts are KYC-gated. POST /users/kyc/verify-bvn submits a Nigerian Bank Verification\n    Number; POST /users/kyc/verify-kyc submits corporate documents and shareholder identity records\n    (firstName, lastName, email, phoneNumber, id) with document URLs previously obtained from\n    PUT /users/upload.\n  operations:\n    - addBvn\n    - verifyKyc\n    - uploadFile\n  jurisdiction: Nigeria (BVN is a Central Bank of Nigeria identifier)\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: >-\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404 on every\n  Cardtonic host (see\
  \ well-known/cardtonic-well-known.yml). There is no OAuth surface to describe.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardtonic/refs/heads/main/authentication/cardtonic-authentication.yml
summary_line: 3 schemes
tags:
- Africa
- Bill Payments
- eSIM
- Finance
- Fintech
- Gift Cards
- Ghana
- Nigeria
- Payments
- Virtual Dollar Cards
---
