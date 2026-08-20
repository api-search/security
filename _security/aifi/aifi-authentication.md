---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Aifi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- deviceCode
- ciba
overview: AiFi secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, deviceCode, and ciba flow(s).
provider_name: AiFi
provider_slug: aifi
scheme_count: 1
schemes:
- capabilities:
    backchannel_logout: true
    claims_parameter: true
    dynamic_client_registration: true
    frontchannel_logout: true
    mtls_bound_tokens: true
    mtls_endpoint_aliases: true
    par: true
    par_required: false
    pkce: true
    pkce_methods:
    - plain
    - S256
    request_object_signing: true
    request_uri_registration_required: true
  client_authentication:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  endpoints:
    authorization: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth
    backchannel_authentication: https://auth.aifi.com/realms/aifi/protocol/openid-connect/ext/ciba/auth
    device_authorization: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth/device
    end_session: https://auth.aifi.com/realms/aifi/protocol/openid-connect/logout
    introspection: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token/introspect
    jwks: https://auth.aifi.com/realms/aifi/protocol/openid-connect/certs
    pushed_authorization_request: https://auth.aifi.com/realms/aifi/protocol/openid-connect/ext/par/request
    registration: https://auth.aifi.com/realms/aifi/clients-registrations/openid-connect
    revocation: https://auth.aifi.com/realms/aifi/protocol/openid-connect/revoke
    token: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token
    userinfo: https://auth.aifi.com/realms/aifi/protocol/openid-connect/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_signing_algs:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  issuer: https://auth.aifi.com/realms/aifi
  name: aifi-keycloak
  openIdConnectUrl: https://auth.aifi.com/realms/aifi/.well-known/openid-configuration
  provider: Keycloak
  sources:
  - well-known/aifi-openid-configuration.json
  type: openIdConnect
slug: aifi-authentication
source_filename: aifi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.aifi.com/realms/aifi/.well-known/openid-configuration\ndocs: null\nnote: >-\n  AiFi publishes no public OpenAPI, so no securitySchemes could be derived from a\n  spec. This profile is built entirely from the one authentication document AiFi\n  does serve anonymously — the OpenID Connect Discovery 1.0 metadata for its\n  Keycloak realm `aifi`, saved verbatim at\n  well-known/aifi-openid-configuration.json. That realm is the identity provider in\n  front of docs.aifi.com (client_id `docs-oidc-client`) and partners.aifi.com. The\n  authentication model used by the OASIS retailer APIs themselves is not published\n  publicly and is NOT asserted here.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - password\n  - deviceCode\n  - ciba\n  spec_derived: false\nschemes:\n- name: aifi-keycloak\n  type: openIdConnect\n  openIdConnectUrl:\
  \ https://auth.aifi.com/realms/aifi/.well-known/openid-configuration\n  issuer: https://auth.aifi.com/realms/aifi\n  provider: Keycloak\n  sources:\n  - well-known/aifi-openid-configuration.json\n  endpoints:\n    authorization: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth\n    token: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token\n    userinfo: https://auth.aifi.com/realms/aifi/protocol/openid-connect/userinfo\n    jwks: https://auth.aifi.com/realms/aifi/protocol/openid-connect/certs\n    introspection: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token/introspect\n    revocation: https://auth.aifi.com/realms/aifi/protocol/openid-connect/revoke\n    end_session: https://auth.aifi.com/realms/aifi/protocol/openid-connect/logout\n    registration: https://auth.aifi.com/realms/aifi/clients-registrations/openid-connect\n    device_authorization: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth/device\n    pushed_authorization_request:\
  \ https://auth.aifi.com/realms/aifi/protocol/openid-connect/ext/par/request\n    backchannel_authentication: https://auth.aifi.com/realms/aifi/protocol/openid-connect/ext/ciba/auth\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  client_authentication:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  capabilities:\n    pkce: true\n    pkce_methods:\n    - plain\n    - S256\n    par: true\n    par_required: false\n    mtls_bound_tokens: true\n    mtls_endpoint_aliases: true\n    backchannel_logout: true\n    frontchannel_logout: true\n    dynamic_client_registration: true\n    request_object_signing: true\n    request_uri_registration_required: true\n    claims_parameter: true\n  id_token_signing_algs:\n  - RS256\n  - RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n\
  \  - ES256\n  - ES384\n  - ES512\n  - HS256\n  - HS384\n  - HS512\nobserved_clients:\n- client_id: docs-oidc-client\n  host: docs.aifi.com\n  scope: openid email profile\n  evidence: 302 Location header on https://docs.aifi.com/\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.aifi.com/realms/aifi/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aifi/refs/heads/main/authentication/aifi-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Computer-Vision
- Retail
- Autonomous Checkout
- Spatial Intelligence
- Artificial Intelligence
- Analytics
- Identity
- Fraud Prevention
- Point-of-Sale
---
