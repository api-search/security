---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Express Scripts Holding Authentication
name_suffix: Authentication
oauth_flows: []
overview: Express Scripts Holding declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Express Scripts Holding
provider_slug: express-scripts-holding
scheme_count: 3
schemes:
- endpoints:
    authorization: https://p1-express-scripts.okta.com/oauth2/default/v1/authorize
    device_authorization: https://p1-express-scripts.okta.com/oauth2/default/v1/device/authorize
    end_session: https://p1-express-scripts.okta.com/oauth2/default/v1/logout
    introspection: https://p1-express-scripts.okta.com/oauth2/default/v1/introspect
    jwks: https://p1-express-scripts.okta.com/oauth2/default/v1/keys
    pushed_authorization_request: https://p1-express-scripts.okta.com/oauth2/default/v1/par
    registration: https://p1-express-scripts.okta.com/oauth2/v1/clients
    revocation: https://p1-express-scripts.okta.com/oauth2/default/v1/revoke
    token: https://p1-express-scripts.okta.com/oauth2/default/v1/token
    userinfo: https://p1-express-scripts.okta.com/oauth2/default/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id: esrx-oidc
  id_token_encryption:
    algs:
    - RSA-OAEP-256
    - RSA-OAEP-384
    - RSA-OAEP-512
    enc:
    - A256GCM
    supported: true
  id_token_signing_algs:
  - RS256
  issuer: https://p1-express-scripts.okta.com/oauth2/default
  openIdConnectUrl: https://p.login.developer.express-scripts.com/oauth2/default/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    note: S256 only — the plain challenge method is not offered.
    supported: true
  protocol: OpenID Connect 1.0
  provider: Okta
  sender_constrained_tokens:
    dpop: true
    dpop_algs:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    mtls: false
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  vanity_issuer: https://p.login.developer.express-scripts.com/oauth2/default
- grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id: esrx-oidc-org
  issuer: https://p.login.developer.express-scripts.com
  note: The Okta org-level authorization server. It additionally advertises the client_credentials grant, which the /oauth2/default server does not — the machine-to-machine path for partner integrations.
  openIdConnectUrl: https://p.login.developer.express-scripts.com/.well-known/openid-configuration
  protocol: OpenID Connect 1.0
  provider: Okta
  type: openIdConnect
- applies_to:
  - https://api.express-scripts.io
  - https://api-sandbox.express-scripts.io
  bearer_format: JWT
  evidence:
  - status: 401
    url: https://api.express-scripts.io/
  - status: 401
    url: https://api-sandbox.express-scripts.io/
  id: esrx-gateway
  note: Both gateway hosts answer HTTP 401 "401 - Unauthorized" to every anonymous request, including /.well-known/* paths. The gateway authenticates before it routes. The token issuer is the Okta estate above; the exact header contract is not published anywhere public.
  scheme: bearer
  type: http
slug: express-scripts-holding-authentication
source_filename: express-scripts-holding-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  https://p.login.developer.express-scripts.com/oauth2/default/.well-known/openid-configuration\n  (HTTP 200, application/json) plus the developer portal's own deployed runtime\n  configuration, read from https://developer.express-scripts.com/assets/index-F-3lEwAf.js\nnote: >-\n  Express Scripts publishes no OpenAPI, so no securityScheme block could be read.\n  This profile is built entirely from documents the provider serves anonymously:\n  two OAuth 2.0 / OpenID Connect discovery documents and the client configuration\n  the portal ships in its own JavaScript bundle. Nothing here is inferred from prose.\nsummary: >-\n  A single OAuth 2.0 / OpenID Connect estate fronted by Express Scripts' own Okta\n  tenant. Every API surface sits behind the same authorization server; the portal\n  itself is an OIDC relying party using authorization code + PKCE.\nschemes:\n  - id: esrx-oidc\n    type: openIdConnect\n    protocol: OpenID\
  \ Connect 1.0\n    openIdConnectUrl: https://p.login.developer.express-scripts.com/oauth2/default/.well-known/openid-configuration\n    issuer: https://p1-express-scripts.okta.com/oauth2/default\n    vanity_issuer: https://p.login.developer.express-scripts.com/oauth2/default\n    provider: Okta\n    endpoints:\n      authorization: https://p1-express-scripts.okta.com/oauth2/default/v1/authorize\n      token: https://p1-express-scripts.okta.com/oauth2/default/v1/token\n      userinfo: https://p1-express-scripts.okta.com/oauth2/default/v1/userinfo\n      jwks: https://p1-express-scripts.okta.com/oauth2/default/v1/keys\n      introspection: https://p1-express-scripts.okta.com/oauth2/default/v1/introspect\n      revocation: https://p1-express-scripts.okta.com/oauth2/default/v1/revoke\n      end_session: https://p1-express-scripts.okta.com/oauth2/default/v1/logout\n      device_authorization: https://p1-express-scripts.okta.com/oauth2/default/v1/device/authorize\n      pushed_authorization_request:\
  \ https://p1-express-scripts.okta.com/oauth2/default/v1/par\n      registration: https://p1-express-scripts.okta.com/oauth2/v1/clients\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    pkce:\n      supported: true\n      methods:\n        - S256\n      note: S256 only — the plain challenge method is not offered.\n    sender_constrained_tokens:\n      dpop: true\n      dpop_algs:\n        - RS256\n        - RS384\n        - RS512\n        - ES256\n        - ES384\n        - ES512\n      mtls: false\n    id_token_signing_algs:\n      - RS256\n    id_token_encryption:\n      supported: true\n      algs:\n        - RSA-OAEP-256\n        - RSA-OAEP-384\n        - RSA-OAEP-512\n    \
  \  enc:\n        - A256GCM\n  - id: esrx-oidc-org\n    type: openIdConnect\n    protocol: OpenID Connect 1.0\n    openIdConnectUrl: https://p.login.developer.express-scripts.com/.well-known/openid-configuration\n    issuer: https://p.login.developer.express-scripts.com\n    provider: Okta\n    note: >-\n      The Okta org-level authorization server. It additionally advertises the\n      client_credentials grant, which the /oauth2/default server does not — the\n      machine-to-machine path for partner integrations.\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n  - id: esrx-gateway\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to:\n      - https://api.express-scripts.io\n      - https://api-sandbox.express-scripts.io\n    note: >-\n      Both gateway hosts answer HTTP 401 \"401\
  \ - Unauthorized\" to every anonymous\n      request, including /.well-known/* paths. The gateway authenticates before it\n      routes. The token issuer is the Okta estate above; the exact header contract\n      is not published anywhere public.\n    evidence:\n      - url: https://api.express-scripts.io/\n        status: 401\n      - url: https://api-sandbox.express-scripts.io/\n        status: 401\nclient_registration:\n  dynamic: true\n  endpoint: https://p1-express-scripts.okta.com/oauth2/v1/clients\n  spec: RFC 7591\n  note: >-\n    A registration_endpoint is advertised in the discovery document. It was NOT\n    exercised — no client was registered. Presence is read from the document only.\nportal_client:\n  note: >-\n    The developer portal's own OIDC client, read verbatim from its deployed bundle.\n    A public client id is not a secret; no credential is recorded here.\n  client_id: 0oa6fdn7jjmwwEue54h7\n  redirect_uri: https://developer.express-scripts.com/login/callback\n  pkce_enabled:\
  \ true\n  scopes:\n    - openid\n    - address\n    - email\n    - phone\n    - profile\n    - esrx.default\nworkforce_idp:\n  issuer: https://cigna.okta.com/oauth2/default\n  redirect_uri: https://internal.developer.express-scripts.com/callback\n  note: >-\n    A second, internal-only relying party for Cigna workforce sign-in. Recorded for\n    completeness; it is not a partner-facing surface.\ngaps:\n  - No OpenAPI is published, so no per-operation security requirements can be read.\n  - >-\n    No /.well-known/oauth-protected-resource (RFC 9728) is served on either gateway\n    host, so an agent cannot discover the authorization server from the resource.\n  - The bearer-token header contract for api.express-scripts.io is not publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-scripts-holding/refs/heads/main/authentication/express-scripts-holding-authentication.yml
summary_line: 3 schemes
tags:
- Health
- Healthcare
- Pharmacy
- Pharmacy Benefit Management
- Prescriptions
- Claims
- Fortune 100
---
