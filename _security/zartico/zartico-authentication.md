---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Zartico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zartico declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Zartico
provider_slug: zartico
scheme_count: 4
schemes:
- dpop_signing_algs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  dynamic_client_registration: true
  endpoints:
    authorization: https://login.zartico.com/oauth2/v1/authorize
    device_authorization: https://login.zartico.com/oauth2/v1/device/authorize
    end_session: https://login.zartico.com/oauth2/v1/logout
    introspection: https://login.zartico.com/oauth2/v1/introspect
    jwks: https://login.zartico.com/oauth2/v1/keys
    pushed_authorization_request: advertised
    registration: https://login.zartico.com/oauth2/v1/clients
    revocation: https://login.zartico.com/oauth2/v1/revoke
    token: https://login.zartico.com/oauth2/v1/token
    userinfo: https://login.zartico.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:okta:params:oauth:grant-type:otp
  - urn:okta:params:oauth:grant-type:oob
  id: okta-oidc-login
  id_token_encryption_alg:
  - RSA-OAEP-256
  - RSA-OAEP-384
  - RSA-OAEP-512
  id_token_signing_alg:
  - RS256
  issuer: https://login.zartico.com
  note: Dynamic client registration and the introspection/revocation endpoints are advertised in the discovery document. They were NOT exercised - this record asserts only what the document declares.
  openIdConnectUrl: https://login.zartico.com/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    supported: true
  provider: Okta
  surface: Zartico Identity (login.zartico.com)
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- dpop_signing_algs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  dynamic_client_registration: true
  endpoints:
    authorization: https://platform.zartico.com/oauth2/v1/authorize
    device_authorization: https://platform.zartico.com/oauth2/v1/device/authorize
    end_session: https://platform.zartico.com/oauth2/v1/logout
    introspection: https://platform.zartico.com/oauth2/v1/introspect
    jwks: https://platform.zartico.com/oauth2/v1/keys
    registration: https://platform.zartico.com/oauth2/v1/clients
    revocation: https://platform.zartico.com/oauth2/v1/revoke
    token: https://platform.zartico.com/oauth2/v1/token
    userinfo: https://platform.zartico.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  id: okta-oidc-platform
  id_token_signing_alg:
  - RS256
  issuer: https://platform.zartico.com
  note: A narrower authorization server than login.zartico.com - no CIBA, no Okta OOB/OTP grants, no pushed authorization request endpoint advertised.
  openIdConnectUrl: https://platform.zartico.com/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    supported: true
  provider: Okta
  surface: Zartico Platform (platform.zartico.com)
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- id: ogc-anonymous
  note: The OGC read surface requires NO authentication. GetCapabilities for WMS 1.3.0, WFS 2.0.0 and WCS 2.0.1 all returned HTTP 200 to an anonymous, unauthenticated request, and both the WMS and WCS capabilities documents declare Fees "none" and AccessConstraints "none".
  surface: Zartico GeoServer OGC Web Services (geoserver.zartico.com)
  type: none
- id: geoserver-rest-admin
  note: https://geoserver.zartico.com/geoserver/rest returned HTTP 401 Unauthorized to an anonymous request. This is GeoServer's built-in administrative REST API, which is protected. It was probed once, unauthenticated, and not pursued further - no credentials of any kind were used or attempted.
  scheme: basic
  surface: GeoServer REST configuration API (geoserver.zartico.com/geoserver/rest)
  type: http
slug: zartico-authentication
source_filename: zartico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://login.zartico.com/.well-known/openid-configuration (200),\n  https://login.zartico.com/.well-known/oauth-authorization-server (200),\n  https://platform.zartico.com/.well-known/openid-configuration (200),\n  https://platform.zartico.com/.well-known/oauth-authorization-server (200),\n  https://geoserver.zartico.com/geoserver/ows?service=WMS&request=GetCapabilities (200, anonymous),\n  https://geoserver.zartico.com/geoserver/rest (401),\n  https://www.zartico.com/security (200)\nnote: |\n  Zartico publishes no developer authentication guide, no API-key issuance flow and no token\n  documentation. Everything below was read from live discovery documents and live probe\n  responses, not from prose. Two distinct auth postures coexist on the estate.\nschemes:\n  - id: okta-oidc-login\n    type: openIdConnect\n    surface: Zartico Identity (login.zartico.com)\n    openIdConnectUrl: https://login.zartico.com/.well-known/openid-configuration\n\
  \    issuer: https://login.zartico.com\n    provider: Okta\n    endpoints:\n      authorization: https://login.zartico.com/oauth2/v1/authorize\n      token: https://login.zartico.com/oauth2/v1/token\n      userinfo: https://login.zartico.com/oauth2/v1/userinfo\n      jwks: https://login.zartico.com/oauth2/v1/keys\n      introspection: https://login.zartico.com/oauth2/v1/introspect\n      revocation: https://login.zartico.com/oauth2/v1/revoke\n      end_session: https://login.zartico.com/oauth2/v1/logout\n      device_authorization: https://login.zartico.com/oauth2/v1/device/authorize\n      registration: https://login.zartico.com/oauth2/v1/clients\n      pushed_authorization_request: advertised\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n      - urn:okta:params:oauth:grant-type:otp\n      - urn:okta:params:oauth:grant-type:oob\n\
  \    pkce:\n      supported: true\n      methods: [S256]\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    id_token_signing_alg: [RS256]\n    id_token_encryption_alg: [RSA-OAEP-256, RSA-OAEP-384, RSA-OAEP-512]\n    dpop_signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512]\n    dynamic_client_registration: true\n    note: >-\n      Dynamic client registration and the introspection/revocation endpoints are advertised in the\n      discovery document. They were NOT exercised - this record asserts only what the document\n      declares.\n  - id: okta-oidc-platform\n    type: openIdConnect\n    surface: Zartico Platform (platform.zartico.com)\n    openIdConnectUrl: https://platform.zartico.com/.well-known/openid-configuration\n    issuer: https://platform.zartico.com\n    provider: Okta\n    endpoints:\n      authorization: https://platform.zartico.com/oauth2/v1/authorize\n  \
  \    token: https://platform.zartico.com/oauth2/v1/token\n      userinfo: https://platform.zartico.com/oauth2/v1/userinfo\n      jwks: https://platform.zartico.com/oauth2/v1/keys\n      introspection: https://platform.zartico.com/oauth2/v1/introspect\n      revocation: https://platform.zartico.com/oauth2/v1/revoke\n      end_session: https://platform.zartico.com/oauth2/v1/logout\n      device_authorization: https://platform.zartico.com/oauth2/v1/device/authorize\n      registration: https://platform.zartico.com/oauth2/v1/clients\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n    pkce:\n      supported: true\n      methods: [S256]\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    id_token_signing_alg: [RS256]\n    dpop_signing_algs: [RS256,\
  \ RS384, RS512, ES256, ES384, ES512]\n    dynamic_client_registration: true\n    note: >-\n      A narrower authorization server than login.zartico.com - no CIBA, no Okta OOB/OTP grants,\n      no pushed authorization request endpoint advertised.\n  - id: ogc-anonymous\n    type: none\n    surface: Zartico GeoServer OGC Web Services (geoserver.zartico.com)\n    note: >-\n      The OGC read surface requires NO authentication. GetCapabilities for WMS 1.3.0, WFS 2.0.0\n      and WCS 2.0.1 all returned HTTP 200 to an anonymous, unauthenticated request, and both the\n      WMS and WCS capabilities documents declare Fees \"none\" and AccessConstraints \"none\".\n  - id: geoserver-rest-admin\n    type: http\n    scheme: basic\n    surface: GeoServer REST configuration API (geoserver.zartico.com/geoserver/rest)\n    note: >-\n      https://geoserver.zartico.com/geoserver/rest returned HTTP 401 Unauthorized to an anonymous\n      request. This is GeoServer's built-in administrative REST API, which\
  \ is protected. It was\n      probed once, unauthenticated, and not pursued further - no credentials of any kind were\n      used or attempted.\nobservations:\n  - >-\n    No API key, bearer token or personal-access-token issuance is documented anywhere on\n    www.zartico.com or support.zartico.com.\n  - >-\n    https://www.zartico.com/security states that hardware 2-factor authentication is required for\n    all Zartico staff and that customer dashboards and portals are password-protected. It\n    documents no customer-facing API authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zartico/refs/heads/main/authentication/zartico-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Travel
- Tourism
- Destination Marketing
- Location Intelligence
- Geospatial
- Analytics
- Data
- Business Intelligence
- OGC
---
