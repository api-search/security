---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Accessfintech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- deviceCode
overview: AccessFintech secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, and deviceCode flow(s).
provider_name: AccessFintech
provider_slug: accessfintech
scheme_count: 2
schemes:
- code_challenge_methods:
  - S256
  endpoints:
    authorization: https://login.accessfintech.com/oauth2/v1/authorize
    device_authorization: https://login.accessfintech.com/oauth2/v1/device/authorize
    end_session: https://login.accessfintech.com/oauth2/v1/logout
    introspection: https://login.accessfintech.com/oauth2/v1/introspect
    jwks: https://login.accessfintech.com/oauth2/v1/keys
    pushed_authorization_request: https://login.accessfintech.com/oauth2/v1/par
    registration: https://login.accessfintech.com/oauth2/v1/clients
    revocation: https://login.accessfintech.com/oauth2/v1/revoke
    token: https://login.accessfintech.com/oauth2/v1/token
    userinfo: https://login.accessfintech.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:okta:params:oauth:grant-type:otp
  - urn:okta:params:oauth:grant-type:oob
  id_token_signing_alg_values:
  - RS256
  issuer: https://login.accessfintech.com
  name: openid-connect
  openIdConnectUrl: https://login.accessfintech.com/.well-known/openid-configuration
  request_object_signing_alg_values:
  - HS256
  - HS384
  - HS512
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  request_parameter_supported: true
  response_types:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  source: probed
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- app_routes:
  - /api/auth/login
  - /api/auth/logout
  - /api/auth/sso
  description: The Synergy web application authenticates against the Okta org's Authentication API (POST /api/v1/authn) and then carries a session cookie, with an anti-CSRF token echoed on every request as the x-csrf-token header and the acting organization supplied as x-context-org-id.
  headers:
    correlation: x-correlation-id
    csrf: x-csrf-token
    organization_context: x-context-org-id
  name: synergy-session
  session_endpoints:
  - POST https://login.accessfintech.com/api/v1/authn
  - DELETE https://login.accessfintech.com/api/v1/sessions/me
  source: https://api.accessfintech.com/assets/index-Cxc8YJZl.js and https://api.accessfintech.com/assets/apollo-client-nEoXJmCU.js (public production bundle)
  type: cookie
slug: accessfintech-authentication
source_filename: accessfintech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://login.accessfintech.com/.well-known/openid-configuration\ndocs: https://www.accessfintech.com/platform/\nnote: >-\n  AccessFintech publishes no OpenAPI, so this profile is not derived from a spec. It is\n  probed directly from the OpenID Connect discovery document the company's identity host\n  serves anonymously, and corroborated by the authentication code in the Synergy web\n  application's own public production JavaScript bundle.\n\nsummary:\n  types: [openIdConnect, oauth2]\n  identity_provider: Okta (customer-branded org at login.accessfintech.com)\n  issuer: https://login.accessfintech.com\n  oauth2_flows: [authorizationCode, implicit, refreshToken, password, deviceCode]\n  pkce: true\n  pkce_methods: [S256]\n  dpop: true\n  par: true\n  dynamic_client_registration: true\n  mtls: false\n  api_key: false\n  enterprise_sso: >-\n    SSO/SAML is advertised on the platform page as a customer-configurable option;\n  \
  \  the Synergy app exposes an /api/auth/sso route.\n\nschemes:\n  - name: openid-connect\n    type: openIdConnect\n    openIdConnectUrl: https://login.accessfintech.com/.well-known/openid-configuration\n    issuer: https://login.accessfintech.com\n    source: probed\n    endpoints:\n      authorization: https://login.accessfintech.com/oauth2/v1/authorize\n      token: https://login.accessfintech.com/oauth2/v1/token\n      userinfo: https://login.accessfintech.com/oauth2/v1/userinfo\n      jwks: https://login.accessfintech.com/oauth2/v1/keys\n      registration: https://login.accessfintech.com/oauth2/v1/clients\n      introspection: https://login.accessfintech.com/oauth2/v1/introspect\n      revocation: https://login.accessfintech.com/oauth2/v1/revoke\n      end_session: https://login.accessfintech.com/oauth2/v1/logout\n      device_authorization: https://login.accessfintech.com/oauth2/v1/device/authorize\n      pushed_authorization_request: https://login.accessfintech.com/oauth2/v1/par\n\
  \    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:okta:params:oauth:grant-type:otp\n      - urn:okta:params:oauth:grant-type:oob\n    response_types: [code, id_token, code id_token, code token, id_token token, code id_token token]\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    code_challenge_methods: [S256]\n    id_token_signing_alg_values: [RS256]\n    subject_types: [public]\n    request_parameter_supported: true\n    request_object_signing_alg_values: [HS256, HS384, HS512, RS256, RS384, RS512, ES256, ES384, ES512]\n\n  - name: synergy-session\n    type: cookie\n    description: >-\n      The Synergy web application authenticates against the Okta org's Authentication API\n      (POST /api/v1/authn) and then carries a session cookie, with an anti-CSRF\
  \ token\n      echoed on every request as the x-csrf-token header and the acting organization\n      supplied as x-context-org-id.\n    source: >-\n      https://api.accessfintech.com/assets/index-Cxc8YJZl.js and\n      https://api.accessfintech.com/assets/apollo-client-nEoXJmCU.js (public production bundle)\n    session_endpoints:\n      - POST https://login.accessfintech.com/api/v1/authn\n      - DELETE https://login.accessfintech.com/api/v1/sessions/me\n    app_routes:\n      - /api/auth/login\n      - /api/auth/logout\n      - /api/auth/sso\n    headers:\n      csrf: x-csrf-token\n      organization_context: x-context-org-id\n      correlation: x-correlation-id\n\ngated: true\ngated_note: >-\n  There is no public developer registration path. Credentials for the Synergy API surface\n  are issued to onboarded network members; the OIDC metadata above is the only part of the\n  authentication contract that is publicly readable.\n\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n    -\
  \ url: https://login.accessfintech.com/.well-known/openid-configuration\n      status: 200\n    - url: https://login.accessfintech.com/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://api.accessfintech.com/assets/index-Cxc8YJZl.js\n      status: 200\n    - url: https://api.accessfintech.com/api/docs\n      status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accessfintech/refs/heads/main/authentication/accessfintech-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Financial Services
- Capital Markets
- Post-Trade
- Settlement
- Data Networks
- Reconciliation
- Fintech
- GraphQL
---
