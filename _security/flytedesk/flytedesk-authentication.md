---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Flytedesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlyteDesk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FlyteDesk
provider_slug: flytedesk
scheme_count: 1
schemes:
- bearer_format: JWT
  description: The application authenticates with a JWT. The endpoint's access-control-expose-headers advertises X-JwtBearerToken, and access-control-allow-headers accepts Authorization, X-Auth-Token and appsessionid, which is how the SPA presents it. There is no self-service way for a third party to obtain one — see credential_issuance below.
  evidence:
    access_control_allow_headers: Content-Type, X-Auth-Token, Origin, appsessionid, Authorization, AppVersion, Content-Disposition, x-playwright-test
    access_control_expose_headers: X-JwtBearerToken, AppVersion, AppVersionMismatch, Content-Disposition
    http_status: 200
    url: https://api.app.flytedesk.com/api/graphql
  header: Authorization
  id: jwt_bearer_session
  location: header
  scheme: bearer
  type: http
slug: flytedesk-authentication
source_filename: flytedesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: graphql/flytedesk-graphql.graphql + live response headers from https://api.app.flytedesk.com/api/graphql\nnote: >-\n  Derived from the introspected GraphQL schema and the live CORS/response headers on the\n  endpoint. FlyteDesk publishes no authentication documentation of any kind — there is no\n  developer portal, no API reference and no auth page to search — so everything below is\n  observed behaviour, not a documented contract. There is NO API-key programme, NO OAuth\n  2.0 authorization server (/.well-known/oauth-authorization-server 404s on every host)\n  and NO OpenID Connect discovery document.\nauth_scheme_count: 1\nschemes:\n- id: jwt_bearer_session\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  location: header\n  header: Authorization\n  description: >-\n    The application authenticates with a JWT. The endpoint's\n    access-control-expose-headers advertises X-JwtBearerToken, and\n    access-control-allow-headers\
  \ accepts Authorization, X-Auth-Token and appsessionid,\n    which is how the SPA presents it. There is no self-service way for a third party to\n    obtain one — see credential_issuance below.\n  evidence:\n    url: https://api.app.flytedesk.com/api/graphql\n    http_status: 200\n    access_control_expose_headers: X-JwtBearerToken, AppVersion, AppVersionMismatch, Content-Disposition\n    access_control_allow_headers: Content-Type, X-Auth-Token, Origin, appsessionid, Authorization, AppVersion, Content-Disposition, x-playwright-test\nsession:\n  cookie: session-uuid\n  attributes: httponly; path=/; Max-Age=3600\n  credentials_mode: access-control-allow-credentials true\n  note: A one-hour session-uuid cookie is set on every request, including anonymous ones.\ncredential_issuance:\n  self_service: false\n  mechanism: >-\n    Credentials are created through the product, not a developer console. The schema\n    exposes loginUserMutation, sendResetPasswordEmailMutation, resetPasswordMutation,\n\
  \    registerUserFromBuyerInvite and registerUserFromSupplierInvite — account creation is\n    invite-driven, initiated by FlyteDesk or an existing buyer/supplier.\n  developer_console: null\n  api_keys: false\n  oauth2: false\n  oidc: false\n  mtls: false\ngating_behaviour:\n  introspection: anonymous, HTTP 200 — the full schema is readable without credentials\n  data: >-\n    gated but soft — an anonymous `{ me { id } }` returns HTTP 200 with\n    `{\"data\":{\"me\":null}}` rather than an authorization error, so unauthorized access is\n    signalled as a null resolution rather than a 401/403 or a GraphQL error extension.\ncors:\n  allow_origin: https://app.flytedesk.com\n  allow_credentials: true\n  allow_methods: POST, GET, OPTIONS, PATCH, PUT, DELETE\n  note: >-\n    A single hard-coded allowed origin. Browser-based third-party clients are excluded by\n    design; this is a first-party application backend.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flytedesk/refs/heads/main/authentication/flytedesk-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Advertising
- Media
- Campus Media
- College Advertising
- Marketing
- AdTech
- GraphQL
- Media Buying
- Higher Education
---
