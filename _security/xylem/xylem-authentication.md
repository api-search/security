---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Xylem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xylem declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Xylem
provider_slug: xylem
scheme_count: 5
schemes:
- description: OpenID Connect Discovery 1.0 metadata for the Xylem Cloud realm. Authorization Code, Client Credentials, Refresh Token, Device Code, JWT Bearer, Token Exchange, UMA ticket and CIBA grants are all advertised.
  id: xcloud-oidc
  openIdConnectUrl: https://cloud.xylem.com/xcloud/auth/realms/xcloud/.well-known/openid-configuration
  type: openIdConnect
- authorization_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/auth
  flow: authorizationCode
  id: xcloud-oauth2-authorization-code
  pkce: true
  pkce_methods:
  - S256
  - plain
  refresh_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token
  token_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token
  type: oauth2
- flow: clientCredentials
  id: xcloud-oauth2-client-credentials
  note: 'Machine-to-machine grant is advertised, and a service_account scope is offered — the shape an integration or an agent would use. Client registration is not open: the dynamic registration endpoint requires an initial access token.'
  token_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token
  type: oauth2
- device_authorization_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/auth/device
  flow: deviceCode
  id: xcloud-oauth2-device-code
  token_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token
  type: oauth2
- id: xcloud-mtls
  note: tls_client_certificate_bound_access_tokens is true and tls_client_auth is an accepted token endpoint auth method (RFC 8705). mtls_endpoint_aliases are published.
  type: mutualTLS
slug: xylem-authentication
source_filename: xylem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://cloud.xylem.com/xcloud/auth/realms/xcloud/.well-known/openid-configuration\ndocs: https://cloud.xylem.com/xcloud/sso/\nnote: >-\n  Derived from the ONE machine-readable authentication document Xylem publishes\n  anonymously: the OpenID Connect discovery document for the Xylem Cloud (xCloud)\n  Keycloak realm, fetched HTTP 200 on 2026-09-04 and saved verbatim at\n  well-known/xylem-openid-configuration.json. Xylem publishes no developer-facing\n  authentication guide and no API reference; everything below is read out of the\n  discovery document itself, not out of prose. There is no public API contract to\n  attach these schemes to, so no securityScheme mapping is asserted.\nprovider: Xylem\nidentity_platform: Keycloak (self-hosted on cloud.xylem.com)\nissuer: https://cloud.xylem.com/xcloud/auth/realms/xcloud\nrealm: xcloud\npublic_client_hint:\n  source: https://cloud.xylem.com/xcloud/sso/\n  note: >-\n    The Xylem Cloud\
  \ sign-in page declares its own browser client configuration inline\n    (realm \"xcloud\", responseType \"token id_token\", scope \"openid email profile\") and\n    names a first-party API base of https://cloud.xylem.com/xcloud/v1/users/. That path\n    returns HTTP 401 UNAUTHORIZED_ERROR unauthenticated, confirming a live, token-guarded\n    REST surface behind this issuer.\nschemes:\n  - type: openIdConnect\n    id: xcloud-oidc\n    openIdConnectUrl: https://cloud.xylem.com/xcloud/auth/realms/xcloud/.well-known/openid-configuration\n    description: >-\n      OpenID Connect Discovery 1.0 metadata for the Xylem Cloud realm. Authorization\n      Code, Client Credentials, Refresh Token, Device Code, JWT Bearer, Token Exchange,\n      UMA ticket and CIBA grants are all advertised.\n  - type: oauth2\n    id: xcloud-oauth2-authorization-code\n    flow: authorizationCode\n    authorization_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/auth\n    token_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token\n\
  \    refresh_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token\n    pkce: true\n    pkce_methods: [S256, plain]\n  - type: oauth2\n    id: xcloud-oauth2-client-credentials\n    flow: clientCredentials\n    token_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token\n    note: >-\n      Machine-to-machine grant is advertised, and a service_account scope is offered —\n      the shape an integration or an agent would use. Client registration is not open:\n      the dynamic registration endpoint requires an initial access token.\n  - type: oauth2\n    id: xcloud-oauth2-device-code\n    flow: deviceCode\n    device_authorization_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/auth/device\n    token_url: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token\n  - type: mutualTLS\n    id: xcloud-mtls\n    note: >-\n      tls_client_certificate_bound_access_tokens is true and\
  \ tls_client_auth is an\n      accepted token endpoint auth method (RFC 8705). mtls_endpoint_aliases are published.\nendpoints:\n  authorization: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/auth\n  token: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token\n  userinfo: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/userinfo\n  jwks: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/certs\n  introspection: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/token/introspect\n  revocation: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/revoke\n  end_session: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/logout\n  registration: https://cloud.xylem.com/xcloud/auth/realms/xcloud/clients-registrations/openid-connect\n  pushed_authorization_request: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/ext/par/request\n\
  \  backchannel_authentication: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/ext/ciba/auth\n  device_authorization: https://cloud.xylem.com/xcloud/auth/realms/xcloud/protocol/openid-connect/auth/device\ntoken_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\ngrant_types:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\ntoken_format: JWT\nid_token_signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512, EdDSA, HS256, HS384, HS512]\ndpop_supported: true\nclaims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - auth_time\n  - name\n  - given_name\n  - family_name\n\
  \  - preferred_username\n  - email\n  - acr\n  - azp\n  - nonce\ngaps:\n  - No published developer authentication guide, key-issuance page, or API reference.\n  - >-\n    No OpenAPI or other contract to bind these schemes to, so an integrator can obtain a\n    token model from discovery but cannot learn which operations it unlocks.\n  - >-\n    Legacy grants (implicit, resource owner password) remain enabled on the realm\n    alongside the modern ones.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/authentication/xylem-authentication.yml
summary_line: 5 schemes
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
---
