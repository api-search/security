---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rallyware Authentication
name_suffix: Authentication
oauth_flows:
- password
- refreshToken
overview: Rallyware secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refreshToken flow(s).
provider_name: Rallyware
provider_slug: rallyware
scheme_count: 4
schemes:
- flow: password
  name: OAuth2Password
  request_body:
    grant_type: password
    password: end-user password
    username: end-user login (email)
  response_body:
    access_token: bearer token
    is_activated: boolean — whether the user account is approved
    is_email_verified: boolean — whether the user email is verified
    refresh_token: token for the refresh_token grant
  source: lib/module/auth/default-auth-strategy.js
  sources:
  - '@rallyware/sdk-react-native-components@1.2.1'
  token_url: /oauth/v2/token
  token_url_note: Relative to the tenant host. Absolute form is https://{tenant}.rallyware.com/oauth/v2/token. The /oauth/v2/ path is the signature of Symfony FOSOAuthServerBundle.
  type: oauth2
- flow: refreshToken
  name: OAuth2RefreshToken
  request_body:
    grant_type: refresh_token
    refresh_token: the refresh_token from a prior grant
  source: lib/module/auth/refresh-token-auth-strategy.js
  sources:
  - '@rallyware/sdk-react-native-components@1.2.1'
  token_url: /oauth/v2/token
  type: oauth2
- description: Every authenticated call carries the access_token from /oauth/v2/token as a bearer token. Set on axios.defaults.headers.common.Authorization.
  format: Bearer {access_token}
  in: header
  name: BearerToken
  parameter_name: Authorization
  scheme: bearer
  source: lib/module/services/rallyware-api-service.js (setAuthData)
  sources:
  - '@rallyware/sdk-react-native-components@1.2.1'
  type: http
- description: A tenant-specific SSO token-exchange endpoint. The SDK ships one concrete implementation, NuskinOktaAuthStrategy, which POSTs {okta_token} to /sdk/okta_login and receives the same access_token/refresh_token envelope as the password grant. This confirms Rallyware supports per-customer enterprise SSO federation into its API, brokered server-side rather than via standard OIDC. Rallyware publishes no generic/documented form of this endpoint — the Nu Skin strategy is the only published example.
  flow: tokenExchange
  name: TenantSSOExchange
  request_body:
    okta_token: an Okta-issued token obtained by the host application
  source: lib/module/auth/nuskin-okta-auth-strategy.js
  sources:
  - '@rallyware/sdk-react-native-components@1.2.1'
  token_url: /sdk/okta_login
  type: oauth2
slug: rallyware-authentication
source_filename: rallyware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: >-\n  npm @rallyware/sdk-react-native-components@1.2.1 — lib/module/auth/*.js and\n  lib/module/services/rallyware-api-service.js (first-party, published by Rallyware)\ndocs: https://www.npmjs.com/package/@rallyware/sdk-react-native-components\nnote: >-\n  Rallyware publishes no developer portal and no OpenAPI. This profile is derived\n  from Rallyware's own published React Native SDK, which contains the complete\n  authentication implementation for the Rallyware tenant API. Every scheme, URL,\n  grant and header below is read verbatim out of that package — nothing is inferred\n  or invented. OWNERSHIP: the package is under the @rallyware npm scope, its\n  repository is github.com/rallyware/sdk-react-native-components, its npm author is\n  \"rallyware\", and its README names Rallyware-operated hosts, so the contract\n  belongs to this company.\n\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [password,\
  \ refreshToken]\n  bearer: true\n  mtls: false\n  openid_connect: false\n  discovery_document: none\n  scopes_published: false\n\nschemes:\n- name: OAuth2Password\n  type: oauth2\n  flow: password\n  token_url: /oauth/v2/token\n  token_url_note: >-\n    Relative to the tenant host. Absolute form is\n    https://{tenant}.rallyware.com/oauth/v2/token. The /oauth/v2/ path is the\n    signature of Symfony FOSOAuthServerBundle.\n  request_body:\n    grant_type: password\n    username: end-user login (email)\n    password: end-user password\n  response_body:\n    access_token: bearer token\n    refresh_token: token for the refresh_token grant\n    is_activated: boolean — whether the user account is approved\n    is_email_verified: boolean — whether the user email is verified\n  source: lib/module/auth/default-auth-strategy.js\n  sources: ['@rallyware/sdk-react-native-components@1.2.1']\n\n- name: OAuth2RefreshToken\n  type: oauth2\n  flow: refreshToken\n  token_url: /oauth/v2/token\n  request_body:\n\
  \    grant_type: refresh_token\n    refresh_token: the refresh_token from a prior grant\n  source: lib/module/auth/refresh-token-auth-strategy.js\n  sources: ['@rallyware/sdk-react-native-components@1.2.1']\n\n- name: BearerToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: \"Bearer {access_token}\"\n  description: >-\n    Every authenticated call carries the access_token from /oauth/v2/token as a\n    bearer token. Set on axios.defaults.headers.common.Authorization.\n  source: lib/module/services/rallyware-api-service.js (setAuthData)\n  sources: ['@rallyware/sdk-react-native-components@1.2.1']\n\n- name: TenantSSOExchange\n  type: oauth2\n  flow: tokenExchange\n  token_url: /sdk/okta_login\n  description: >-\n    A tenant-specific SSO token-exchange endpoint. The SDK ships one concrete\n    implementation, NuskinOktaAuthStrategy, which POSTs {okta_token} to\n    /sdk/okta_login and receives the same access_token/refresh_token envelope as the\n\
  \    password grant. This confirms Rallyware supports per-customer enterprise SSO\n    federation into its API, brokered server-side rather than via standard OIDC.\n    Rallyware publishes no generic/documented form of this endpoint — the Nu Skin\n    strategy is the only published example.\n  request_body:\n    okta_token: an Okta-issued token obtained by the host application\n  source: lib/module/auth/nuskin-okta-auth-strategy.js\n  sources: ['@rallyware/sdk-react-native-components@1.2.1']\n\ntoken_lifecycle:\n  refresh_trigger: >-\n    HTTP 401 on any authenticated request. The SDK's axios response interceptor\n    retries the original request exactly once after exchanging the refresh_token; if\n    the refresh also fails, all auth state is cleared and the error is rejected.\n  retry_guard: _retry flag on the axios request config (single retry, no loop)\n  source: lib/module/services/rallyware-api-service.js (interceptors.response)\n\nauthorization_gates:\n  description: >-\n    Beyond\
  \ token validity, the SDK treats the API as unavailable unless the\n    authenticated principal passes two account-state gates returned by the token\n    response.\n  gates:\n  - field: is_activated\n    meaning: the user account has been approved by the tenant administrator\n  - field: is_email_verified\n    meaning: the user email address has been verified\n  computed_as: isInitialized && accessToken && refreshToken && isUserApproved && isUserEmailVerified\n\nanonymous_endpoints:\n  description: >-\n    Two endpoints are called before authentication and require no token.\n  endpoints:\n  - GET /api/public/config\n  - GET /api/public/translation/catalogue/{langCode}\n  note: >-\n    Both are tenant-scoped and were NOT anonymously reachable from the public\n    internet during this pass — no Rallyware tenant host answers to an unauthenticated\n    caller (see x-coverage in apis.yml).\n\nscopes:\n  published: false\n  note: >-\n    The password grant is issued without a scope parameter\
  \ and no scope or permission\n    reference is published anywhere. Authorization is enforced by tenant role and\n    account state, not by OAuth scopes, so no scopes/ artifact is emitted rather\n    than an empty one.\n\ngaps:\n- No /.well-known/oauth-authorization-server (RFC 8414) metadata is served.\n- No /.well-known/openid-configuration is served; this is OAuth2 only, not OIDC.\n- No client_credentials or authorization_code grant is published — the only grants\n  Rallyware documents are resource-owner password credentials and refresh_token.\n  RFC 6749 §4.3 discourages the password grant and OAuth 2.1 removes it entirely.\n- No public documentation of client_id/client_secret registration for the token\n  endpoint; the SDK omits them, implying a public client per tenant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rallyware/refs/heads/main/authentication/rallyware-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Company
- Sales Enablement
- Workforce Enablement
- Learning and Development
- Performance Management
- Gamification
- Direct Selling
- Enterprise Software
---
