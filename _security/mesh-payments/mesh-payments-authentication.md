---
api_key_in: []
auth_types:
- http
- oauth2
- custom-hmac
description: ''
kind: authentication
layout: security
method: searched
name: Mesh Payments Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
- tokenExchange
overview: Mesh Payments secures its APIs with http, oauth2, and custom-hmac across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, deviceCode, and tokenExchange flow(s).
provider_name: Mesh Payments
provider_slug: mesh-payments
scheme_count: 3
schemes:
- algorithm: HMAC-SHA256
  description: Mesh's help center states the REST API supports HMAC-SHA256 request signing. First-party reference implementations were published in Postman, Python 3+, Node.js 10+, Java 8+, .NET C# and PHP.
  name: HMAC-SHA256 request signing
  note: the exact canonical string, header names and clock-skew window are documented only on the gated developers portal, so they are not recorded here.
  scheme: hmac
  source: https://github.com/mesh-payments/hmac-auth-examples
  source_status: archived 2026-05-24, read-only
  type: custom
- description: Machine-to-machine access token issuance for server-side API clients.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.meshpayments.com/as/token
  name: OAuth 2.0 client credentials
  source: https://api.meshpayments.com/.well-known/oauth-authorization-server
  type: oauth2
- code_challenge_methods_supported:
  - S256
  description: Mesh runs a full OAuth 2.0 authorization server with OIDC discovery. It is the authorization server named by the MCP endpoint's RFC 9728 protected-resource metadata.
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://api.meshpayments.com/as/authorize
    device_authorization: https://api.meshpayments.com/oauth2/device_authorization
    end_session: https://api.meshpayments.com/connect/logout
    introspection: https://api.meshpayments.com/oauth2/introspect
    jwks: https://api.meshpayments.com/as/jwks
    registration: https://api.meshpayments.com/as/register
    revocation: https://api.meshpayments.com/oauth2/revoke
    token: https://api.meshpayments.com/as/token
    userinfo: https://api.meshpayments.com/as/userinfo
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.meshpayments.com
  name: OAuth 2.0 / OpenID Connect authorization server
  openIdConnectUrl: https://api.meshpayments.com/.well-known/openid-configuration
  source: https://api.meshpayments.com/.well-known/openid-configuration
  tls_client_certificate_bound_access_tokens: true
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  type: openIdConnect
slug: mesh-payments-authentication
source_filename: mesh-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://kb.meshpayments.com/support/integrators-corner/does-mesh-offer-restful-api-integration/\ndocs: https://developers.meshpayments.com\ndocs_note: the full authentication reference and code samples live on the Mesh Developers\n  Portal, which is served behind CloudFront HTTP Basic authentication (401 to the public);\n  everything below is derived from the publicly readable help-center article, the archived\n  first-party HMAC example repository, and the live OAuth/OIDC discovery documents\n  on api.meshpayments.com\nsummary:\n  types:\n  - http\n  - oauth2\n  - custom-hmac\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - deviceCode\n  - tokenExchange\n  api_key_in: []\nschemes:\n- name: HMAC-SHA256 request signing\n  type: custom\n  scheme: hmac\n  algorithm: HMAC-SHA256\n  description: Mesh's help center states the REST API supports HMAC-SHA256 request\n    signing. First-party reference implementations\
  \ were published in Postman, Python\n    3+, Node.js 10+, Java 8+, .NET C# and PHP.\n  source: https://github.com/mesh-payments/hmac-auth-examples\n  source_status: archived 2026-05-24, read-only\n  note: the exact canonical string, header names and clock-skew window are documented\n    only on the gated developers portal, so they are not recorded here.\n- name: OAuth 2.0 client credentials\n  type: oauth2\n  description: Machine-to-machine access token issuance for server-side API clients.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.meshpayments.com/as/token\n  source: https://api.meshpayments.com/.well-known/oauth-authorization-server\n- name: OAuth 2.0 / OpenID Connect authorization server\n  type: openIdConnect\n  openIdConnectUrl: https://api.meshpayments.com/.well-known/openid-configuration\n  issuer: https://api.meshpayments.com\n  description: Mesh runs a full OAuth 2.0 authorization server with OIDC discovery.\n    It is the authorization server named by\
  \ the MCP endpoint's RFC 9728 protected-resource\n    metadata.\n  endpoints:\n    authorization: https://api.meshpayments.com/as/authorize\n    token: https://api.meshpayments.com/as/token\n    device_authorization: https://api.meshpayments.com/oauth2/device_authorization\n    userinfo: https://api.meshpayments.com/as/userinfo\n    jwks: https://api.meshpayments.com/as/jwks\n    revocation: https://api.meshpayments.com/oauth2/revoke\n    introspection: https://api.meshpayments.com/oauth2/introspect\n    registration: https://api.meshpayments.com/as/register\n    end_session: https://api.meshpayments.com/connect/logout\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\n\
  \  code_challenge_methods_supported:\n  - S256\n  dpop_signing_alg_values_supported:\n  - RS256\n  - RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\n  tls_client_certificate_bound_access_tokens: true\n  id_token_signing_alg_values_supported:\n  - RS256\n  source: https://api.meshpayments.com/.well-known/openid-configuration\nnotable:\n- PKCE S256 is the only code challenge method advertised.\n- DPoP (RFC 9449) sender-constrained tokens are supported across nine signing algorithms.\n- mTLS client authentication (RFC 8705) is supported both with a CA-issued and a self-signed\n  certificate, and certificate-bound access tokens are enabled.\n- Private-key JWT and client-secret JWT client authentication are supported alongside\n  the basic/post forms.\n- RFC 7591 dynamic client registration is exposed at /as/register.\n- Token exchange (RFC 8693) is an advertised grant type.\n- Platform sign-in also supports SAML SSO with passwordless access and enforces\
  \ MFA\n  per https://meshpayments.com/security-is-our-priority/.\nx-evidence:\n- fetched: '2026-08-04'\n  url: https://api.meshpayments.com/.well-known/openid-configuration\n  http_status: 200\n- fetched: '2026-08-04'\n  url: https://api.meshpayments.com/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-04'\n  url: https://kb.meshpayments.com/support/integrators-corner/does-mesh-offer-restful-api-integration/\n  http_status: 200\n- fetched: '2026-08-04'\n  url: https://developers.meshpayments.com\n  http_status: 401\n  note: WWW-Authenticate Basic\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-payments/refs/heads/main/authentication/mesh-payments-authentication.yml
summary_line: http/oauth2/custom-hmac · 3 schemes
tags:
- Company
- Payments
- Spend Management
- Expense Management
- Corporate Cards
- Travel
- Accounts Payable
- Fintech
- Card Issuing
- Accounting Automation
---
