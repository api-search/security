---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Result Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Result secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Result
provider_slug: result
scheme_count: 4
schemes:
- caveat: 'The docs note in passing that an end-user HTTP call carries `Authorization: Bearer <publishable key>`, not an x-api-key header — while explicitly telling developers not to hand-roll HTTP at all.'
  description: The publishable client key. Ships in the browser bundle by design — the provider states plainly that anyone can read it out of a shipped frontend. It is what @resultdev/sdk uses for every application call.
  env_var: NEXT_PUBLIC_BACKEND_ANON_KEY
  format: Bearer <publishable key>
  header: Authorization
  in: header
  name: publishable-anon-key
  plane: backend-credentials
  public: true
  type: apiKey
  what_protects_data:
  - Row-level security. Tables created with a user_id uuid column get an owner policy scoping rows to the signed-in user; RLS is on by default.
  - Signed-in-only writes. Storage uploads and list() reject anonymous callers.
  - Serverless functions as the trust boundary. AI calls and email sends work with the publishable key alone, so anyone holding it can drive spend; the docs direct expensive or sensitive operations into a function.
- description: Full admin control of the backend — schema, migrations, buckets, realtime channel patterns, functions, secrets, payment keys, deployments. Terminal or server-side code only.
  env_var: BACKEND_ADMIN_KEY
  in: header
  name: backend-admin-key
  plane: backend-credentials
  prohibitions:
  - Never in client code.
  - Never in a NEXT_PUBLIC_* variable.
  - Never in the browser.
  - Never as a Result-hosting build variable.
  public: false
  type: apiKey
  used_by: '@resultdev/cli'
- description: Issued at sign-in and attached by the SDK to every database, storage, function and realtime call, which is what makes RLS-scoped tables resolve correctly.
  discovery_call: getPublicAuthConfig() -> data.oAuthProviders
  flow_control:
    default: auto
    modes:
    - redirect
    - popup
    - auto
    note: Google refuses to render inside an iframe, so the SDK detects a framed app and opens a popup instead. redirectTo must share an origin with the page starting the sign-in; a cross-origin value is refused up front with OAUTH_REDIRECT_CROSS_ORIGIN.
  name: end-user-session
  plane: end-user-session
  profiles:
    fields:
    - name
    - avatar_url
    operations:
    - getProfile
    - setProfile
  providers:
  - method: email-password
    note: signUp returns a session immediately; email verification is pre-configured off, so there is no "check your email" stall.
    operations:
    - signUp
    - signInWithPassword
    - signOut
    - sendResetPasswordEmail
    - resetPassword
  - method: oauth
    note: configured on every backend, no client ID to register, no callback route to build
    operation: signInWithOAuth("google")
    provider: google
  - method: oauth
    operation: signInWithOAuth("github")
    provider: github
  scheme: bearer
  session_restore:
    call: getCurrentUser()
    rule: Must be called on mount. onAuthStateChange() reports changes only and never fires for an already-existing session, so it cannot stand in for the restore call.
  token_storage:
    access_token: in memory
    hardened_variant: '''@resultdev/sdk/ssr'' puts the refresh token in an httpOnly cookie the application''s own server writes, which browser JavaScript cannot read. The docs name XSS as a session-theft hole in the default configuration and call the SSR variant the right trade for apps holding something worth stealing.'
    localstorage: deliberately empty — the docs state an empty localStorage never means "signed out", and that sign-in state must be checked with getCurrentUser(), never by reading browser storage
    refresh_token: first-party cookie on the application's own origin, written by the SDK
    requires: SDK 0.7.0 or newer for cookie-based session persistence
  type: http
- dpop_supported: true
  dynamic_client_registration: https://api.descope.com/v1/mgmt/inboundapp/app/P3HVe6On8gLt3t2puHvHToMFQit2/register
  flows:
  - authorizationUrl: https://api.descope.com/oauth2/v1/apps/authorize
    flow: authorizationCode
    refreshUrl: https://api.descope.com/oauth2/v1/apps/token
    revocationUrl: https://api.descope.com/oauth2/v1/apps/revoke
    scopes:
      full-access: Read and write access to the businesses the authenticated account owns.
    tokenUrl: https://api.descope.com/oauth2/v1/apps/token
    userinfoUrl: https://api.descope.com/oauth2/v1/apps/userinfo
  id_token_signing_alg:
  - RS256
  identity_provider: Descope
  issuer: https://api.descope.com/v1/apps/P3HVe6On8gLt3t2puHvHToMFQit2
  jwks_uri: https://api.descope.com/P3HVe6On8gLt3t2puHvHToMFQit2/.well-known/jwks.json
  name: mcp-oauth
  pkce:
  - S256
  plane: mcp-oauth
  protected_resource: https://api.result.dev/mcp
  protected_resource_metadata: https://api.result.dev/.well-known/oauth-protected-resource
  sources:
  - well-known/result-oauth-protected-resource.json
  - well-known/result-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: result-authentication
source_filename: result-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.result.dev/sdk/authentication, https://docs.result.dev/guides/security,\n  https://docs.result.dev/guides/troubleshooting, and the anonymous RFC 9728/RFC 8414\n  metadata at https://api.result.dev/.well-known/oauth-protected-resource\ndocs:\n- https://docs.result.dev/sdk/authentication\n- https://docs.result.dev/guides/security\nnote: >-\n  Result publishes no OpenAPI, so this profile is searched from the provider's own\n  documentation and from live OAuth discovery metadata rather than derived from\n  securitySchemes. There are two distinct authentication planes: credentials that\n  authenticate an APPLICATION to its own Result Backend, and an OAuth 2.1 flow that\n  authenticates a HUMAN OPERATOR (and their agent) to the Result MCP server.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  planes: [backend-credentials, mcp-oauth, end-user-session]\n\
  schemes:\n- name: publishable-anon-key\n  plane: backend-credentials\n  type: apiKey\n  in: header\n  header: Authorization\n  format: 'Bearer <publishable key>'\n  env_var: NEXT_PUBLIC_BACKEND_ANON_KEY\n  public: true\n  description: >-\n    The publishable client key. Ships in the browser bundle by design — the provider states\n    plainly that anyone can read it out of a shipped frontend. It is what @resultdev/sdk\n    uses for every application call.\n  what_protects_data:\n  - Row-level security. Tables created with a user_id uuid column get an owner policy\n    scoping rows to the signed-in user; RLS is on by default.\n  - Signed-in-only writes. Storage uploads and list() reject anonymous callers.\n  - Serverless functions as the trust boundary. AI calls and email sends work with the\n    publishable key alone, so anyone holding it can drive spend; the docs direct expensive\n    or sensitive operations into a function.\n  caveat: >-\n    The docs note in passing that an end-user\
  \ HTTP call carries\n    `Authorization: Bearer <publishable key>`, not an x-api-key header — while explicitly\n    telling developers not to hand-roll HTTP at all.\n- name: backend-admin-key\n  plane: backend-credentials\n  type: apiKey\n  in: header\n  env_var: BACKEND_ADMIN_KEY\n  public: false\n  used_by: '@resultdev/cli'\n  description: >-\n    Full admin control of the backend — schema, migrations, buckets, realtime channel\n    patterns, functions, secrets, payment keys, deployments. Terminal or server-side code\n    only.\n  prohibitions:\n  - Never in client code.\n  - Never in a NEXT_PUBLIC_* variable.\n  - Never in the browser.\n  - Never as a Result-hosting build variable.\n- name: end-user-session\n  plane: end-user-session\n  type: http\n  scheme: bearer\n  description: >-\n    Issued at sign-in and attached by the SDK to every database, storage, function and\n    realtime call, which is what makes RLS-scoped tables resolve correctly.\n  providers:\n  - method: email-password\n\
  \    operations: [signUp, signInWithPassword, signOut, sendResetPasswordEmail, resetPassword]\n    note: >-\n      signUp returns a session immediately; email verification is pre-configured off, so\n      there is no \"check your email\" stall.\n  - method: oauth\n    provider: google\n    operation: signInWithOAuth(\"google\")\n    note: configured on every backend, no client ID to register, no callback route to build\n  - method: oauth\n    provider: github\n    operation: signInWithOAuth(\"github\")\n  discovery_call: getPublicAuthConfig() -> data.oAuthProviders\n  token_storage:\n    access_token: in memory\n    refresh_token: first-party cookie on the application's own origin, written by the SDK\n    localstorage: >-\n      deliberately empty — the docs state an empty localStorage never means \"signed out\",\n      and that sign-in state must be checked with getCurrentUser(), never by reading browser\n      storage\n    requires: SDK 0.7.0 or newer for cookie-based session persistence\n\
  \    hardened_variant: >-\n      '@resultdev/sdk/ssr' puts the refresh token in an httpOnly cookie the application's own\n      server writes, which browser JavaScript cannot read. The docs name XSS as a\n      session-theft hole in the default configuration and call the SSR variant the right\n      trade for apps holding something worth stealing.\n  session_restore:\n    call: getCurrentUser()\n    rule: >-\n      Must be called on mount. onAuthStateChange() reports changes only and never fires for\n      an already-existing session, so it cannot stand in for the restore call.\n  flow_control:\n    modes: [redirect, popup, auto]\n    default: auto\n    note: >-\n      Google refuses to render inside an iframe, so the SDK detects a framed app and opens a\n      popup instead. redirectTo must share an origin with the page starting the sign-in;\n      a cross-origin value is refused up front with OAUTH_REDIRECT_CROSS_ORIGIN.\n  profiles:\n    operations: [getProfile, setProfile]\n    fields:\
  \ [name, avatar_url]\n- name: mcp-oauth\n  plane: mcp-oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.descope.com/oauth2/v1/apps/authorize\n    tokenUrl: https://api.descope.com/oauth2/v1/apps/token\n    refreshUrl: https://api.descope.com/oauth2/v1/apps/token\n    revocationUrl: https://api.descope.com/oauth2/v1/apps/revoke\n    userinfoUrl: https://api.descope.com/oauth2/v1/apps/userinfo\n    scopes:\n      full-access: Read and write access to the businesses the authenticated account owns.\n  issuer: https://api.descope.com/v1/apps/P3HVe6On8gLt3t2puHvHToMFQit2\n  jwks_uri: https://api.descope.com/P3HVe6On8gLt3t2puHvHToMFQit2/.well-known/jwks.json\n  protected_resource: https://api.result.dev/mcp\n  protected_resource_metadata: https://api.result.dev/.well-known/oauth-protected-resource\n  dynamic_client_registration: https://api.descope.com/v1/mgmt/inboundapp/app/P3HVe6On8gLt3t2puHvHToMFQit2/register\n  pkce: [S256]\n  dpop_supported:\
  \ true\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  identity_provider: Descope\n  sources: [well-known/result-oauth-protected-resource.json, well-known/result-oauth-authorization-server.json]\naccount_identity:\n  note: >-\n    The Terms of Service state a Google account is required to sign in to Result itself\n    (distinct from the end-user auth an application built on Result offers its own users).\nx-evidence:\n- url: https://docs.result.dev/sdk/authentication\n  status: 200\n- url: https://docs.result.dev/guides/security\n  status: 200\n- url: https://api.result.dev/.well-known/oauth-protected-resource\n  status: 200\n- url: https://api.descope.com/v1/apps/P3HVe6On8gLt3t2puHvHToMFQit2/.well-known/oauth-authorization-server\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/result/refs/heads/main/authentication/result-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Business Operations
- Software-as-a-Service
- Entrepreneurship
- Payments
- Marketing
- No-Code
- Startups
- Artificial Intelligence
- Backend as a Service
- MCP
- Agents
- Database
- Authentication
- Storage
- Serverless
- Real-Time
---
