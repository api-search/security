---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: probed
name: Countertack Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
- implicit
- password
- refresh_token
- device_code
- token_exchange
- uma_ticket
- ciba
overview: CounterTack secures its APIs with openIdConnect, oauth2, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, client_credentials, implicit, password, refresh_token, device_code, token_exchange, uma_ticket, and ciba flow(s).
provider_name: CounterTack
provider_slug: countertack
scheme_count: 2
schemes:
- capabilities:
    authorization_response_iss_parameter: true
    back_channel_logout: true
    dpop: false
    front_channel_logout: true
    jarm_response_modes: true
    mtls_bound_access_tokens: true
    mtls_endpoint_aliases: true
    pushed_authorization_requests: supported
    request_object: true
    require_pushed_authorization_requests: false
    uma2: true
  claims:
  - aud
  - sub
  - iss
  - auth_time
  - name
  - given_name
  - family_name
  - preferred_username
  - email
  - acr
  endpoints:
    authorization: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth
    backchannel_authentication: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/ext/ciba/auth
    device_authorization: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth/device
    end_session: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/logout
    introspection: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token/introspect
    jwks: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/certs
    pushed_authorization_request: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/ext/par/request
    registration: https://login.gosecure.net/realms/gosec-titan/clients-registrations/openid-connect
    revocation: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/revoke
    token: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token
    userinfo: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/userinfo
  id_token_signing_algs:
  - RS256
  - ES256
  - ES384
  - ES512
  - PS256
  - PS384
  - PS512
  - RS384
  - RS512
  - HS256
  - HS384
  - HS512
  - EdDSA
  issuer: https://login.gosecure.net/realms/gosec-titan
  name: gosec-titan
  openIdConnectUrl: https://login.gosecure.net/realms/gosec-titan/.well-known/openid-configuration
  pkce_methods:
  - plain
  - S256
  provider: Keycloak
  sources:
  - well-known/countertack-gosec-titan-openid-configuration.json
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
- name: titan-console
  note: The Titan web console at https://titan.gosecure.net/ redirects unauthenticated users into the same realm; the observed login form posts to https://login.gosecure.net/realms/gosec-titan/login-actions/authenticate with client_id=titan and redirect_uri https://titan.gosecure.net/oauth2/callback.
  sources:
  - probe: https://titan.gosecure.net/
    status: 200
  type: openIdConnect
slug: countertack-authentication
source_filename: countertack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://login.gosecure.net/realms/gosec-titan/.well-known/openid-configuration\ndocs: null\nnote: 'Derived entirely from the anonymously-served OpenID Connect discovery document\n  of the GoSecure Titan Keycloak realm (gosec-titan). There is no public OpenAPI for\n  the CounterTack/GoSecure Titan API — api.gosecure.net returns 401 on every path —\n  so no securityScheme could be derived from a spec, and none was invented. GoSecure\n  publishes no public authentication documentation page that could be found.'\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - device_code\n  - token_exchange\n  - uma_ticket\n  - ciba\nschemes:\n- name: gosec-titan\n  type: openIdConnect\n  provider: Keycloak\n  issuer: https://login.gosecure.net/realms/gosec-titan\n  openIdConnectUrl: https://login.gosecure.net/realms/gosec-titan/.well-known/openid-configuration\n\
  \  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n  endpoints:\n    authorization: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth\n    token: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token\n    userinfo: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/userinfo\n    jwks: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/certs\n    introspection: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token/introspect\n    revocation: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/revoke\n    end_session: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/logout\n    registration: https://login.gosecure.net/realms/gosec-titan/clients-registrations/openid-connect\n    device_authorization: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth/device\n    pushed_authorization_request: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/ext/par/request\n\
  \    backchannel_authentication: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/ext/ciba/auth\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  pkce_methods:\n  - plain\n  - S256\n  id_token_signing_algs:\n  - RS256\n  - ES256\n  - ES384\n  - ES512\n  - PS256\n  - PS384\n  - PS512\n  - RS384\n  - RS512\n  - HS256\n  - HS384\n  - HS512\n  - EdDSA\n  claims:\n  - aud\n  - sub\n  - iss\n  - auth_time\n  - name\n  - given_name\n  - family_name\n  - preferred_username\n  - email\n  - acr\n  capabilities:\n    mtls_bound_access_tokens: true\n    mtls_endpoint_aliases: true\n    pushed_authorization_requests: supported\n    require_pushed_authorization_requests: false\n    dpop: false\n    request_object: true\n    jarm_response_modes: true\n    front_channel_logout: true\n    back_channel_logout: true\n    authorization_response_iss_parameter: true\n    uma2: true\n- name:\
  \ titan-console\n  type: openIdConnect\n  note: 'The Titan web console at https://titan.gosecure.net/ redirects unauthenticated\n    users into the same realm; the observed login form posts to\n    https://login.gosecure.net/realms/gosec-titan/login-actions/authenticate with\n    client_id=titan and redirect_uri https://titan.gosecure.net/oauth2/callback.'\n  sources:\n  - probe: https://titan.gosecure.net/\n    status: 200\napi_surface:\n  host: https://api.gosecure.net\n  anonymous_status: 401\n  www_authenticate: null\n  note: 'The API host returns 401 with no WWW-Authenticate header on every path,\n    including with a bearer token present, so the exact credential form the Titan API\n    accepts cannot be confirmed anonymously. The Keycloak realm above is the documented\n    identity provider for the platform; whether the API accepts realm-issued bearer\n    tokens is not publicly verifiable.'\nx-evidence:\n  fetched: '2026-08-11'\n  probes:\n  - url: https://login.gosecure.net/realms/gosec-titan/.well-known/openid-configuration\n\
  \    status: 200\n  - url: https://login.gosecure.net/realms/gosec-titan/.well-known/uma2-configuration\n    status: 200\n  - url: https://api.gosecure.net/\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countertack/refs/heads/main/authentication/countertack-authentication.yml
summary_line: openIdConnect/oauth2/mutualTLS · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Endpoint Security
- Endpoint Detection and Response
- Managed Detection and Response
- Threat Detection
- Incident Response
- SIEM
---
