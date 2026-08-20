---
api_key_in: []
api_specs:
- filename: adready-cpxi-kickstart-openapi.yml
  format: yaml
  label: Digital Remedy Platform (Kickstart) API
  slug: digital-remedy-platform-kickstart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adready-cpxi/refs/heads/main/openapi/adready-cpxi-kickstart-openapi.yml
auth_types:
- session-jwt
description: ''
kind: authentication
layout: security
method: derived
name: Adready Cpxi Authentication
name_suffix: Authentication
oauth_flows: []
overview: AdReady (CPXi) secures its APIs with session-jwt across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AdReady (CPXi)
provider_slug: adready-cpxi
scheme_count: 1
schemes:
- bearer_format: JWT
  declared_in_openapi: false
  description: A session JSON Web Token issued by POST /api/auth/login and managed by the token-controller operations. The spec does not describe where the credential is carried (header vs cookie); the login response is typed only as a bare object, and the browser client sets axios withCredentials true, which is consistent with a cookie-borne session. Confirming the exact carrier requires an authenticated session and was not attempted.
  name: SessionJWT
  scheme: bearer
  sources:
  - openapi/adready-cpxi-kickstart-openapi.yml
  status: undeclared-but-enforced
  type: http
slug: adready-cpxi-authentication
source_filename: adready-cpxi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/adready-cpxi-kickstart-openapi.yml + live unauthenticated probes of https://platform.digitalremedy.com\nnote: >-\n  The published OpenAPI declares NO components.securitySchemes and NO top-level or per-operation\n  security[] requirements, so nothing here is derived from a declared scheme. The auth model below is\n  reconstructed from the authentication and token operations the spec DOES describe, corroborated by\n  live unauthenticated probes: every business path returns HTTP 401 with an empty body, while\n  /version, /health-check, /api/version, /api/theme and /api/config answer 200 anonymously.\n  This gap between the deployed enforcement and the described contract is the finding — an agent\n  reading this spec alone cannot tell that the API requires authentication, or how to obtain a token.\n\nsummary:\n  types:\n  - session-jwt\n  api_key_in: []\n  oauth2_flows: []\n  declared_in_spec: false\n  enforced_at_runtime:\
  \ true\n\nschemes:\n- name: SessionJWT\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  declared_in_openapi: false\n  status: undeclared-but-enforced\n  description: >-\n    A session JSON Web Token issued by POST /api/auth/login and managed by the token-controller\n    operations. The spec does not describe where the credential is carried (header vs cookie); the\n    login response is typed only as a bare object, and the browser client sets\n    axios withCredentials true, which is consistent with a cookie-borne session. Confirming the exact\n    carrier requires an authenticated session and was not attempted.\n  sources:\n  - openapi/adready-cpxi-kickstart-openapi.yml\n\ncredential_operations:\n- operationId: authenticateUser\n  method: post\n  path: /api/auth/login\n  purpose: Exchange email + password for a session token\n  request_schema: LoginRequest\n  request_fields:\n  - email (string, format email, required)\n  - password (string, required)\n  query_parameters:\n  - name:\
  \ app\n    required: true\n    type: integer\n    note: Application discriminator; the spec documents no enumeration of valid values.\n- operationId: authenticatePlusUser\n  method: post\n  path: /api/auth/plus_login\n  purpose: Login path for the legacy AdReady+ (plus.adready.com) application\n- operationId: loginAhUser\n  method: post\n  path: /api/auth/loginC360User\n  purpose: Login path for Compulse 360 (C360) users, following the Compulse / Digital Remedy combination\n- operationId: refreshToken\n  method: get\n  path: /api/token/refresh\n  purpose: Refresh the session token\n  response_schema: ApiResponseTokenWrapper\n- operationId: parseJwtToken\n  method: get\n  path: /api/token/parse\n  purpose: Parse and inspect the current JWT\n- operationId: removeJwtToken\n  method: delete\n  path: /api/token/remove\n  purpose: Invalidate the session token (logout)\n\npassword_lifecycle_operations:\n- {operationId: createPassword, method: post, path: /api/auth/forgot_password}\n- {operationId:\
  \ createPassword_1, method: post, path: /api/auth/create_password}\n- {operationId: ResetPassword, method: post, path: /api/auth/reset_password}\n- {operationId: validateResetPasswordToken, method: post, path: /api/auth/validate_token}\n- {operationId: sendVerificationEmail, method: post, path: /api/sendVerificationEmail}\n\ndelegated_analytics_tokens:\n  note: >-\n    The API mints short-lived tokens for embedded third-party analytics surfaces rather than exposing\n    those systems directly. These are outbound delegation, not inbound API authentication.\n  operations:\n  - {operationId: tableauJwtToken, path: '/api/token/tableau', target: Tableau}\n  - {operationId: tableauJwtTokenByAccount, path: '/api/token/tableau/account/{accountId}', target: Tableau}\n  - {operationId: tableauJwtToken_1, path: '/api/token/tableau/{advertiserId}', target: Tableau}\n  - {operationId: tableauSignInTokenByAdvertiser, path: '/api/token/tableau/sign/{advertiserId}', target: Tableau}\n  - {operationId:\
  \ generateThoughtSpotToken, path: '/api/token/thoughtSpot', target: ThoughtSpot}\n\nanonymous_operations:\n  note: Observed 200 without credentials on 2026-08-12.\n  paths:\n  - {path: /version, status: 200, returns: build metadata (version, git revision, build time)}\n  - {path: /api/version, status: 200, returns: build metadata}\n  - {path: /health-check, status: 200, returns: 'plain text: server is up'}\n  - {path: /api/theme, status: 200, returns: white-label theme CSS}\n  - {path: /api/config, status: 200, returns: client bootstrap configuration}\n  - {path: /v3/api-docs, status: 200, returns: the OpenAPI 3.1 description itself}\n  - {path: /swagger-ui.html, status: 200, returns: Swagger UI}\n\nruntime_evidence:\n- {url: 'https://platform.digitalremedy.com/api/users/1', status: 401, body_length: 0, www_authenticate: absent}\n- {url: 'https://platform.digitalremedy.com/config', status: 401, body_length: 0}\n- {url: 'https://platform.digitalremedy.com/version', status: 200}\n- {url:\
  \ 'https://platform.digitalremedy.com/v3/api-docs', status: 200}\n\ngaps:\n- No securitySchemes declared in the OpenAPI, so no operation states its auth requirement.\n- The 401 response carries no body and no WWW-Authenticate challenge header.\n- Only one operation in 355 documents a 401 response and only one documents a 403.\n- No OAuth 2.0, no OpenID Connect, no API keys, and therefore no scope surface.\n- No public sign-up: credentials are provisioned by Digital Remedy, not self-served.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adready-cpxi/refs/heads/main/authentication/adready-cpxi-authentication.yml
summary_line: session-jwt · 1 scheme
tags:
- Company
- Commerce
- Advertising
- AdTech
- Marketing
- Programmatic
- Media
- Media Planning
- Campaign Management
- Attribution
- Connected TV
- Ad Operations
- Measurements
- Agencies
---
