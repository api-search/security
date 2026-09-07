---
anonymous_access: false
api_key_in: []
auth_types: []
description: Every 4.screen API surface is protected. The whole of api.4screen.com answers HTTP 401 with a {"httpStatus":401,"domain":"SYSTEM","errorCode":"AUTHENTICATION_FAILED"} envelope for anonymous callers. Authentication is OpenID Connect / OAuth 2.0 against a self-hosted Keycloak realm mounted under /auth on the same host, and that realm's discovery document IS served anonymously — so the auth contract is public even though the API contract is not.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 4Screen Authentication
name_suffix: Authentication
oauth_flows: []
overview: 4.screen declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 4.screen
provider_slug: 4screen
scheme_count: 2
schemes:
- description: Full OIDC discovery is published. Clients obtain a bearer JWT from the Keycloak token endpoint and present it to api.4screen.com.
  format: Bearer <JWT>
  header: Authorization
  id: openIdConnect
  in: header
  openIdConnectUrl: https://api.4screen.com/auth/realms/fourscreen/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth 2.0 flows advertised by the realm. client_credentials is the server-to-server mode a partner integration would use; authorization_code with PKCE (S256 advertised) is what the browser portal uses.
  flows:
    authorizationCode:
      authorizationUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth
      refreshUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token
      tokenUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token
    clientCredentials:
      tokenUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token
    deviceCode:
      deviceAuthorizationUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth/device
  id: oauth2
  type: oauth2
slug: 4screen-authentication
source_filename: 4screen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://api.4screen.com/auth/realms/fourscreen/.well-known/openid-configuration\ndocs: null\nname: 4.screen API authentication\ndescription: >-\n  Every 4.screen API surface is protected. The whole of api.4screen.com answers\n  HTTP 401 with a {\"httpStatus\":401,\"domain\":\"SYSTEM\",\"errorCode\":\"AUTHENTICATION_FAILED\"}\n  envelope for anonymous callers. Authentication is OpenID Connect / OAuth 2.0\n  against a self-hosted Keycloak realm mounted under /auth on the same host, and\n  that realm's discovery document IS served anonymously — so the auth contract\n  is public even though the API contract is not.\n\nx-evidence:\n  fetched: '2026-09-05'\n  discovery_url: https://api.4screen.com/auth/realms/fourscreen/.well-known/openid-configuration\n  discovery_status: 200\n  discovery_content_type: application/json;charset=UTF-8\n  saved_verbatim: well-known/4screen-openid-configuration.json\n  anonymous_api_probe:\n    url: https://api.4screen.com/\n\
  \    status: 401\n    body: '{\"httpStatus\":401,\"domain\":\"SYSTEM\",\"errorCode\":\"AUTHENTICATION_FAILED\",\"message\":\"Full authentication is required to access this resource\"}'\n  discovered_via: >-\n    https://portal.4screen.com/config.js (HTTP 200) publishes\n    window.AUTH_URL = 'https://api.4screen.com/auth' and\n    window.AUTH_REALM = 'fourscreen', which is what located the realm path.\n\nprovider:\n  identity_provider: Keycloak\n  self_hosted: true\n  issuer: https://api.4screen.com/auth/realms/fourscreen\n  realm: fourscreen\n  note: >-\n    Keycloak is 4.screen's own deployment on their own API host, not a\n    third-party IDaaS tenant. The public_key and realm metadata are readable at\n    https://api.4screen.com/auth/realms/fourscreen (HTTP 200).\n\nschemes:\n  - id: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://api.4screen.com/auth/realms/fourscreen/.well-known/openid-configuration\n    description: >-\n      Full OIDC discovery is published.\
  \ Clients obtain a bearer JWT from the\n      Keycloak token endpoint and present it to api.4screen.com.\n    in: header\n    header: Authorization\n    format: 'Bearer <JWT>'\n  - id: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 flows advertised by the realm. client_credentials is the\n      server-to-server mode a partner integration would use; authorization_code\n      with PKCE (S256 advertised) is what the browser portal uses.\n    flows:\n      clientCredentials:\n        tokenUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token\n      authorizationCode:\n        authorizationUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth\n        tokenUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token\n        refreshUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token\n      deviceCode:\n        deviceAuthorizationUrl: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth/device\n\
  \nendpoints:\n  issuer: https://api.4screen.com/auth/realms/fourscreen\n  authorization: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth\n  token: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token\n  introspection: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token/introspect\n  userinfo: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/userinfo\n  jwks_uri: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/certs\n  revocation: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/revoke\n  end_session: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/logout\n  device_authorization: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth/device\n  backchannel_authentication: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/ext/ciba/auth\n  pushed_authorization_request: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/ext/par/request\n\
  \  dynamic_client_registration: https://api.4screen.com/auth/realms/fourscreen/clients-registrations/openid-connect\n\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:ietf:params:oauth:grant-type:token-exchange'\n  - 'urn:ietf:params:oauth:grant-type:uma-ticket'\n  - 'urn:openid:params:grant-type:ciba'\n\ntoken_endpoint_auth_methods_supported:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n\ncapabilities:\n  pkce: true\n  pkce_methods: [plain, S256]\n  mtls_client_auth: true\n  mtls_bound_access_tokens: true\n  pushed_authorization_requests: true\n  par_required: false\n  dpop: false\n  dynamic_client_registration: true\n  backchannel_logout: true\n  frontchannel_logout: true\n  request_object_support: true\n  request_uri_registration_required: true\n  claims_parameter_supported: true\n\n\
  id_token_signing_algs:\n  - RS256\n  - RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\n  - EdDSA\n  - HS256\n  - HS384\n  - HS512\n\nclaims_supported: [aud, sub, iss, auth_time, name, given_name, family_name, preferred_username, email, acr]\n\nknown_clients:\n  - client_id: portal\n    surface: https://portal.4screen.com\n    note: >-\n      Public browser client for the 4.screen customer portal, named in the\n      portal's own config.js. Its presence confirms authorization_code is the\n      interactive flow; the partner/OEM integration path is client_credentials.\n\nobservations:\n  - >-\n    Notable weakness in the published posture: the realm still advertises the\n    `implicit` and `password` (Resource Owner Password Credentials) grant types,\n    both of which OAuth 2.0 Security BCP (RFC 9700) says MUST NOT be used. This\n    is Keycloak's default surface rather than a deliberate 4.screen choice, but\n    it is what the discovery document tells\
  \ a client.\n  - >-\n    Notable strength: mutual-TLS client authentication and certificate-bound\n    access tokens (RFC 8705) are both advertised, as are Pushed Authorization\n    Requests (RFC 9126) and private_key_jwt — an unusually complete set for a\n    company of this size, and the pieces a FAPI-grade integration needs.\n  - >-\n    require_pushed_authorization_requests is false, so PAR is available but not\n    enforced.\n\ngaps:\n  - >-\n    No published API reference, so which scope or role each endpoint requires is\n    not documented anywhere public. The scope NAMES are known (see\n    scopes/4screen-scopes.yml) but their operation mapping is not.\n  - >-\n    No documented API-key alternative for server-to-server callers; every\n    integration goes through the OAuth token endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4screen/refs/heads/main/authentication/4screen-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- AdTech
- Automotive
- Mobility
- Connected Vehicle
- In-Car Commerce
- Location
- Navigation
- Marketing
- Germany
---
