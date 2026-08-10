---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Deskera Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Deskera secures its APIs with oauth2, apiKey, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Deskera
provider_slug: deskera
scheme_count: 3
schemes:
- description: Every Deskera endpoint is secured and requires a valid access token passed in the x-access-token request header. The token is a signed JWT (RFC 7519) issued by the Deskera OAuth 2.0 token endpoint or by the sign-in APIs.
  in: header
  name: x-access-token
  parameter_name: x-access-token
  sources:
  - https://deskera.github.io/Developer-Documentation/docs/books/started
  - https://deskera.github.io/Developer-Documentation/docs/crmplus/started
  type: apiKey
- description: Three-legged OAuth 2.0 authorization-code flow. Partners register with Deskera by email to receive a client_id and client_secret, then send users to the Deskera authorization page with response_type=code, scope and client_id; the returned authorization code is exchanged for access_token and refresh_token.
  flows:
  - authorizationUrl: https://oauth.deskera.com/
    flow: authorizationCode
    scopes_documented:
    - read
    - write
    tokenUrl: https://bifrost-us.deskera.com/oauth/token
    token_endpoint_auth: 'HTTP Basic — Authorization: Basic base64(client_id + ":" + client_secret)'
  name: Authorization
  sources:
  - https://deskera.github.io/Developer-Documentation/docs/books/oauthv2
  - https://deskera.github.io/Developer-Documentation/docs/environment/prod
  staging:
    authorizationUrl: https://oauth-staging.deskera.xyz/
    tokenUrl: https://api-staging.deskera.xyz/v2/oauth/token
  type: oauth2
- description: A second security scheme named ApiKeyAuth appears on a subset of documented operations (97 documented operations in the developer docs) alongside the predominant "Authorization" scheme. The docs do not publish the parameter name separately from x-access-token.
  in: header
  name: ApiKeyAuth
  sources:
  - https://deskera.github.io/Developer-Documentation/docs/books/iamapi
  type: apiKey
slug: deskera-authentication
source_filename: deskera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\ndocs:\n- https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\n- https://deskera.github.io/Developer-Documentation/docs/books/authenticationv2\n- https://deskera.github.io/Developer-Documentation/docs/books/setup\n- https://deskera.github.io/Developer-Documentation/docs/environment/prod\nnote: >-\n  Deskera publishes no public OpenAPI/Swagger document — the API host answers\n  HTTP 410 on every Swagger documentation path (see lifecycle/). This profile is\n  therefore searched from the provider's own developer documentation rather than\n  derived from a machine-readable spec.\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  primary_credential: x-access-token request header\nschemes:\n- name: x-access-token\n  type: apiKey\n  in: header\n  parameter_name: x-access-token\n\
  \  description: >-\n    Every Deskera endpoint is secured and requires a valid access token passed in\n    the x-access-token request header. The token is a signed JWT (RFC 7519) issued\n    by the Deskera OAuth 2.0 token endpoint or by the sign-in APIs.\n  sources:\n  - https://deskera.github.io/Developer-Documentation/docs/books/started\n  - https://deskera.github.io/Developer-Documentation/docs/crmplus/started\n- name: Authorization\n  type: oauth2\n  description: >-\n    Three-legged OAuth 2.0 authorization-code flow. Partners register with Deskera\n    by email to receive a client_id and client_secret, then send users to the\n    Deskera authorization page with response_type=code, scope and client_id; the\n    returned authorization code is exchanged for access_token and refresh_token.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.deskera.com/\n    tokenUrl: https://bifrost-us.deskera.com/oauth/token\n    token_endpoint_auth: >-\n      HTTP Basic — Authorization:\
  \ Basic base64(client_id + \":\" + client_secret)\n    scopes_documented:\n    - read\n    - write\n  staging:\n    authorizationUrl: https://oauth-staging.deskera.xyz/\n    tokenUrl: https://api-staging.deskera.xyz/v2/oauth/token\n  sources:\n  - https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\n  - https://deskera.github.io/Developer-Documentation/docs/environment/prod\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  description: >-\n    A second security scheme named ApiKeyAuth appears on a subset of documented\n    operations (97 documented operations in the developer docs) alongside the\n    predominant \"Authorization\" scheme. The docs do not publish the parameter name\n    separately from x-access-token.\n  sources:\n  - https://deskera.github.io/Developer-Documentation/docs/books/iamapi\ntoken_lifecycle:\n  validate_endpoint: GET /v1/iam/token/app/validate\n  refresh: >-\n    refresh_token exchanged at the OAuth token endpoint; the SDK exposes\n    getAppRefreshToken(refreshToken)\n\
  \  expiry: >-\n    access_token is short-lived and can be validated at any time; the docs state it\n    \"is not a permanent token and might become invalid time to time\"\nsign_in_methods:\n- web password sign-in (POST /v1/iam/auth/sign-in/web/sign-in)\n- mobile sign-in with verification (POST /v1/iam/auth/sign-in/mobile, /mobile/verify)\n- email OTP (POST /v1/iam/auth/sign-in/send-otp-mail)\n- multi-factor authentication enable/verify/disable (/web/mfa, /web/mfa-enable, /web/mfa-signin, /web/mfa-status)\n- OIDC sign-in (POST /v1/iam/auth/sign-in/web/oidc-signin)\n- Clerk sign-in (POST /v1/iam/auth/sign-in/web/clerk-signin)\n- Workday sign-in (POST /v1/iam/auth/sign-in/web/workday-signin)\npartner_registration:\n  process: email\n  contact: care@deskera.com\n  required: app name, purpose, company name, email, HTTPS callback URL, public or private use\n  url: https://deskera.github.io/Developer-Documentation/docs/books/setup\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\n\
  \  - https://raw.githubusercontent.com/Deskera/Developer-Documentation/master/docs/books/oauthv2.md\n  - https://raw.githubusercontent.com/Deskera/Developer-Documentation/master/docs/environment/prod.md\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deskera/refs/heads/main/authentication/deskera-authentication.yml
summary_line: oauth2/apiKey/http · 3 schemes
tags:
- Company
- ERP
- Accounting
- CRM
- Human Resources
- Payroll
- Inventory
- Invoicing
- Small Business
- SaaS
---
