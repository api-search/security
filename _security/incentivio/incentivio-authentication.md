---
api_key_in: []
api_specs:
- filename: incentivio-mobile-api-openapi.yml
  format: yaml
  label: Incentivio Mobile & Ordering API
  slug: mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incentivio/refs/heads/main/openapi/incentivio-mobile-api-openapi.yml
- filename: incentivio-admin-api-openapi.yml
  format: yaml
  label: Incentivio Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incentivio/refs/heads/main/openapi/incentivio-admin-api-openapi.yml
auth_types: []
description: 'Incentivio publishes no narrative authentication documentation, and neither OpenAPI definition declares a securityScheme — the springdoc generator emitted none. The auth model was therefore established by probe: both production services answer unauthenticated requests with `WWW-Authenticate: Bearer realm="restservice"`, and both serve RFC 8414 OAuth 2.0 Authorization Server Metadata anonymously at /.well-known/oauth-authorization-server. The metadata is a Spring Authorization Server document describing authorization_code (with PKCE S256), client_credentials, refresh_token, device_code and token-exchange grants. There are two separate issuers, one per audience.'
kind: authentication
layout: security
method: probed
name: Incentivio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Incentivio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Incentivio
provider_slug: incentivio
scheme_count: 2
schemes:
- applies_to:
  - incentivio:mobile-api
  - incentivio:admin-api
  bearer_format: JWT (unverified — token format not published)
  evidence:
  - 'GET https://mobile.incentivio.com/incentivio-mobile-api/useraccounts -> 401, WWW-Authenticate: Bearer realm="restservice"'
  - 'GET https://mobile.incentivio.com/incentivio-mobile-api/loyaltyaccounts -> 401, WWW-Authenticate: Bearer realm="restservice"'
  header: Authorization
  id: bearer-token
  in: header
  note: The 401 body is empty; the reason is carried in the custom response headers incentivio-code and incentivio-message (see conventions/).
  scheme: bearer
  type: http
- applies_to:
  - incentivio:mobile-api
  - incentivio:admin-api
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  id: oauth2
  issuers:
  - audience: guest / ordering apps
    authorization_endpoint: https://order.incentivio.com/issuer/oauth2/authorize
    device_authorization_endpoint: https://order.incentivio.com/issuer/oauth2/device_authorization
    file: well-known/incentivio-mobile-api-oauth-authorization-server.json
    introspection_endpoint: https://order.incentivio.com/issuer/oauth2/introspect
    issuer: https://order.incentivio.com/issuer
    jwks_uri: https://order.incentivio.com/issuer/oauth2/jwks
    revocation_endpoint: https://order.incentivio.com/issuer/oauth2/revoke
    token_endpoint: https://order.incentivio.com/issuer/oauth/token
  - audience: brand operators / admin console
    authorization_endpoint: https://admin.incentivio.com/issuer/oauth2/authorize
    device_authorization_endpoint: https://admin.incentivio.com/issuer/oauth2/device_authorization
    file: well-known/incentivio-admin-api-oauth-authorization-server.json
    introspection_endpoint: https://admin.incentivio.com/issuer/oauth2/introspect
    issuer: https://admin.incentivio.com/issuer
    jwks_uri: https://admin.incentivio.com/issuer/oauth2/jwks
    revocation_endpoint: https://admin.incentivio.com/issuer/oauth2/revoke
    token_endpoint: https://admin.incentivio.com/issuer/oauth/token
  metadata_source: RFC 8414 (/.well-known/oauth-authorization-server)
  mutual_tls: tls_client_certificate_bound_access_tokens is true (RFC 8705), and both tls_client_auth and self_signed_tls_client_auth are offered as client authentication methods — an unusually strong posture for a platform with no public developer program.
  response_types_supported:
  - code
  scopes_note: Neither metadata document publishes a scopes_supported array and neither OpenAPI declares oauth2 flows, so there is no scope registry to harvest. This is why no scopes/ artifact exists for this provider.
  scopes_supported: null
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  type: oauth2
slug: incentivio-authentication
source_filename: incentivio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mobile.incentivio.com/incentivio-mobile-api/.well-known/oauth-authorization-server,\n  https://adminapi.incentivio.com/incentivio-admin-api/.well-known/oauth-authorization-server,\n  live WWW-Authenticate challenges on both API hosts, and the auth operations in\n  openapi/incentivio-mobile-api-openapi.yml\nname: Incentivio authentication profile\ndescription: >-\n  Incentivio publishes no narrative authentication documentation, and neither\n  OpenAPI definition declares a securityScheme — the springdoc generator emitted\n  none. The auth model was therefore established by probe: both production\n  services answer unauthenticated requests with\n  `WWW-Authenticate: Bearer realm=\"restservice\"`, and both serve RFC 8414\n  OAuth 2.0 Authorization Server Metadata anonymously at\n  /.well-known/oauth-authorization-server. The metadata is a Spring\n  Authorization Server document describing authorization_code (with PKCE\
  \ S256),\n  client_credentials, refresh_token, device_code and token-exchange grants.\n  There are two separate issuers, one per audience.\ncaveat: >-\n  The advertised issuer endpoints (order.incentivio.com/issuer/*,\n  admin.incentivio.com/issuer/*) do not resolve to the authorization server from\n  the public edge — both hosts return the single-page-app HTML shell for those\n  paths. The metadata is real and published; the endpoints it names appear to be\n  reachable only from the applications themselves. A third-party developer\n  cannot complete an OAuth flow from this metadata alone.\nschemes:\n  - id: bearer-token\n    type: http\n    scheme: bearer\n    bearer_format: JWT (unverified — token format not published)\n    in: header\n    header: Authorization\n    applies_to:\n      - incentivio:mobile-api\n      - incentivio:admin-api\n    evidence:\n      - 'GET https://mobile.incentivio.com/incentivio-mobile-api/useraccounts -> 401, WWW-Authenticate: Bearer realm=\"restservice\"\
  '\n      - 'GET https://mobile.incentivio.com/incentivio-mobile-api/loyaltyaccounts -> 401, WWW-Authenticate: Bearer realm=\"restservice\"'\n    note: >-\n      The 401 body is empty; the reason is carried in the custom response headers\n      incentivio-code and incentivio-message (see conventions/).\n  - id: oauth2\n    type: oauth2\n    applies_to:\n      - incentivio:mobile-api\n      - incentivio:admin-api\n    metadata_source: RFC 8414 (/.well-known/oauth-authorization-server)\n    issuers:\n      - audience: guest / ordering apps\n        issuer: https://order.incentivio.com/issuer\n        authorization_endpoint: https://order.incentivio.com/issuer/oauth2/authorize\n        token_endpoint: https://order.incentivio.com/issuer/oauth/token\n        device_authorization_endpoint: https://order.incentivio.com/issuer/oauth2/device_authorization\n        introspection_endpoint: https://order.incentivio.com/issuer/oauth2/introspect\n        revocation_endpoint: https://order.incentivio.com/issuer/oauth2/revoke\n\
  \        jwks_uri: https://order.incentivio.com/issuer/oauth2/jwks\n        file: well-known/incentivio-mobile-api-oauth-authorization-server.json\n      - audience: brand operators / admin console\n        issuer: https://admin.incentivio.com/issuer\n        authorization_endpoint: https://admin.incentivio.com/issuer/oauth2/authorize\n        token_endpoint: https://admin.incentivio.com/issuer/oauth/token\n        device_authorization_endpoint: https://admin.incentivio.com/issuer/oauth2/device_authorization\n        introspection_endpoint: https://admin.incentivio.com/issuer/oauth2/introspect\n        revocation_endpoint: https://admin.incentivio.com/issuer/oauth2/revoke\n        jwks_uri: https://admin.incentivio.com/issuer/oauth2/jwks\n        file: well-known/incentivio-admin-api-oauth-authorization-server.json\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n\
  \    response_types_supported:\n      - code\n    code_challenge_methods_supported:\n      - S256\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - tls_client_auth\n      - self_signed_tls_client_auth\n    mutual_tls: >-\n      tls_client_certificate_bound_access_tokens is true (RFC 8705), and both\n      tls_client_auth and self_signed_tls_client_auth are offered as client\n      authentication methods — an unusually strong posture for a platform with no\n      public developer program.\n    scopes_supported: null\n    scopes_note: >-\n      Neither metadata document publishes a scopes_supported array and neither\n      OpenAPI declares oauth2 flows, so there is no scope registry to harvest.\n      This is why no scopes/ artifact exists for this provider.\nfirst_party_login_operations:\n  - operationId: userLogin\n    method: POST\n    path: /users/login\n    api: incentivio:mobile-api\n\
  \  - operationId: userLogin2\n    method: POST\n    path: /users/login2\n    api: incentivio:mobile-api\n  - operationId: authInit\n    method: POST\n    path: /auth/init\n    api: incentivio:mobile-api\n    note: passwordless-auth-controller — initiates a passwordless (phone/email code) sign-in.\n  - operationId: authorizationCode\n    method: GET\n    path: /oauth2/authorizationCode/google\n    api: incentivio:mobile-api\n    note: >-\n      Social sign-in exchange for Google. The ordering web app also loads Apple's\n      appleid.auth.js, so Sign in with Apple is in play on the client side.\n  - operationId: verifyUserAccountEmail\n    method: POST\n    path: /verifyemail\n    api: incentivio:mobile-api\n  - operationId: verifyUserAccountWithCode\n    method: GET\n    path: /verifyUserAccountWithCode\n    api: incentivio:mobile-api\ntenancy:\n  model: >-\n    Authentication alone is not sufficient — every call also has to name the\n    restaurant brand it acts for. The two services\
  \ use different header names for\n    the same idea.\n  headers:\n    - name: CLIENTID\n      api: incentivio:mobile-api\n      operations_declaring_it: 20\n    - name: Inc-Client-Id\n      api: incentivio:admin-api\n      operations_declaring_it: 52\n    - name: Inc-Merchant-Id\n      api: incentivio:admin-api\n      operations_declaring_it: 10\n  path_parameters:\n    - name: clientid\n      note: 121 admin operations and 4 mobile operations carry the tenant in the path.\n    - name: merchantid\n  resolution_operations:\n    - operationId: getClientIdByAlias\n      path: /clientalias/{clientAlias}\n      note: Resolves a brand alias to the CLIENTID value the rest of the API expects.\n    - operationId: getClientDomainByClientAlias\n      path: /clientdomain/byalias\nbot_protection:\n  present: true\n  evidence: recaptcha-controller in the mobile OpenAPI (GET /recaptcha/cache/{clientId})\n  note: reCAPTCHA gating is applied to guest-facing account and order flows.\ndocs: null\ndocs_note:\
  \ >-\n  There is no published authentication guide. apidocs.incentivio.com is an empty\n  Theneo developer portal (zero published projects), and incentivio.com has no\n  developer section.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incentivio/refs/heads/main/authentication/incentivio-authentication.yml
summary_line: 2 schemes
tags:
- Restaurant
- Guest Engagement
- Online Ordering
- Loyalty
- Customer Data Platform
- Marketing Automation
- Analytics
- Reverse ETL
- Restaurant Technology
- Point-of-Sale
- Gift Cards
- Mobile Ordering
---
