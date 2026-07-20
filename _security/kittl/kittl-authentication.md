---
api_key_in: []
auth_types:
- jwt
- oauth2-client
- interactive-device-login
description: ''
kind: authentication
layout: security
method: searched
name: Kittl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kittl secures its APIs with jwt, oauth2-client, and interactive-device-login across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kittl
provider_slug: kittl
scheme_count: 3
schemes:
- description: '`kittl auth login` signs a developer in. It attempts to open a browser and also prints a URL plus a short code that can be completed on another device.'
  human_required: true
  name: cli-session
  non_interactive_note: Token-based non-interactive auth (--non-interactive for login) is documented as not yet supported, so unattended CI publishing is not currently possible.
  non_interactive_supported: false
  source: https://sdk-docs.kittl.dev/getting-started/kittl-cli
  surface: Kittl CLI
  type: interactive-device-login
- description: The app frontend obtains a short-lived Kittl user JWT via `kittl.auth.getUserToken()` and sends it to the app's own backend, which verifies it with @kittl/sdk-backend.
  name: kittl-user-token
  source: https://sdk-docs.kittl.dev/getting-started/sdk-backend
  surface: App frontend to app backend
  type: jwt
  verification:
    audience: appId
    audience_note: appId is used as the JWT audience, so tokens issued for a different app are rejected.
    error: TokenInvalidError (return 401 Unauthorized)
    method: KittlSDK.verifyUserToken(token)
    package: '@kittl/sdk-backend'
    signing_key_cache:
      default: in-memory per SDK instance
      default_max_age_ms: 3600000
      default_max_entries: 5
      pluggable: true
      pluggable_note: A persistent SigningKeyCache can be supplied to reuse keys across restarts and cold starts on edge/serverless backends.
    subject: The verified token's `sub` claim is a pseudonymous per-app user ID — it is not a stable cross-app Kittl user identifier.
- description: An app declares third-party OAuth providers in manifest.json under `config.oauthProviders` and runs the flow through `kittl.auth`, so provider secrets are never exposed in the sandboxed client.
  flows:
  - authorizationUrl: declared per provider in manifest.json (config.oauthProviders.<id>.authorizationUrl)
    flow: authorizationCode
    pkce_note: 'Pass generatePKCE: true to kittl.auth.startAuth; recommended when the provider supports OAuth 2.1 / PKCE.'
    pkce_supported: true
    tokenUrl: declared per provider in manifest.json (config.oauthProviders.<id>.tokenUrl)
  manifest_fields:
  - clientId
  - scope
  - authorizationUrl
  - tokenUrl
  - accessType
  - customFieldMappings
  methods:
  - method: kittl.auth.startAuth
    purpose: Begin the flow; returns an authorization code (and code_verifier with PKCE).
  - method: kittl.auth.exchangeCode
    purpose: Exchange the authorization code for the provider's token response payload.
  - method: kittl.auth.getAuthToken
    purpose: Restore a previously stored token on app reload.
  - method: kittl.auth.getUserToken
    purpose: Obtain the short-lived Kittl user JWT for app-backend verification.
  name: oauth-providers
  redirect_uri: https://app.kittl.com/auth/callback/:appId
  redirect_uri_note: :appId is the app's ID; this must be registered as the callback with the provider.
  role: client
  surface: Sandboxed app to third-party provider
  type: oauth2
slug: kittl-authentication
source_filename: kittl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://sdk-docs.kittl.dev/Guides/Advanced/authentication\ndocs: https://sdk-docs.kittl.dev/Guides/Advanced/authentication\nnotes: >-\n  Derived mechanically-by-script is not possible here — Kittl publishes no OpenAPI, so\n  0-working/derive-authentication.py has no securitySchemes to read. This profile is\n  searched from the published SDK documentation instead. Kittl's app platform has three\n  distinct authentication surfaces, captured separately below: (1) CLI developer login,\n  (2) an app-to-backend user identity token, and (3) an OAuth *client* helper that lets a\n  sandboxed app authenticate against a third-party provider without exposing secrets in\n  the browser. Kittl does not operate a public OAuth authorization server of its own and\n  publishes no /.well-known/openid-configuration or /.well-known/oauth-authorization-server.\nsummary:\n  types:\n  - jwt\n  - oauth2-client\n  - interactive-device-login\n  api_key_in:\
  \ []\n  oauth2_flows:\n  - authorizationCode\n  oauth2_role: client-only\n  authorization_server_published: false\nschemes:\n- name: cli-session\n  surface: Kittl CLI\n  type: interactive-device-login\n  description: >-\n    `kittl auth login` signs a developer in. It attempts to open a browser and also\n    prints a URL plus a short code that can be completed on another device.\n  human_required: true\n  non_interactive_supported: false\n  non_interactive_note: >-\n    Token-based non-interactive auth (--non-interactive for login) is documented as not\n    yet supported, so unattended CI publishing is not currently possible.\n  source: https://sdk-docs.kittl.dev/getting-started/kittl-cli\n- name: kittl-user-token\n  surface: App frontend to app backend\n  type: jwt\n  description: >-\n    The app frontend obtains a short-lived Kittl user JWT via\n    `kittl.auth.getUserToken()` and sends it to the app's own backend, which verifies it\n    with @kittl/sdk-backend.\n  verification:\n  \
  \  package: '@kittl/sdk-backend'\n    method: KittlSDK.verifyUserToken(token)\n    audience: appId\n    audience_note: >-\n      appId is used as the JWT audience, so tokens issued for a different app are\n      rejected.\n    subject: >-\n      The verified token's `sub` claim is a pseudonymous per-app user ID — it is not a\n      stable cross-app Kittl user identifier.\n    error: TokenInvalidError (return 401 Unauthorized)\n    signing_key_cache:\n      default: in-memory per SDK instance\n      default_max_age_ms: 3600000\n      default_max_entries: 5\n      pluggable: true\n      pluggable_note: >-\n        A persistent SigningKeyCache can be supplied to reuse keys across restarts and\n        cold starts on edge/serverless backends.\n  source: https://sdk-docs.kittl.dev/getting-started/sdk-backend\n- name: oauth-providers\n  surface: Sandboxed app to third-party provider\n  type: oauth2\n  role: client\n  description: >-\n    An app declares third-party OAuth providers in manifest.json\
  \ under\n    `config.oauthProviders` and runs the flow through `kittl.auth`, so provider secrets\n    are never exposed in the sandboxed client.\n  flows:\n  - flow: authorizationCode\n    pkce_supported: true\n    pkce_note: >-\n      Pass generatePKCE: true to kittl.auth.startAuth; recommended when the provider\n      supports OAuth 2.1 / PKCE.\n    authorizationUrl: declared per provider in manifest.json (config.oauthProviders.<id>.authorizationUrl)\n    tokenUrl: declared per provider in manifest.json (config.oauthProviders.<id>.tokenUrl)\n  redirect_uri: https://app.kittl.com/auth/callback/:appId\n  redirect_uri_note: ':appId is the app''s ID; this must be registered as the callback with the provider.'\n  manifest_fields:\n  - clientId\n  - scope\n  - authorizationUrl\n  - tokenUrl\n  - accessType\n  - customFieldMappings\n  methods:\n  - method: kittl.auth.startAuth\n    purpose: Begin the flow; returns an authorization code (and code_verifier with PKCE).\n  - method: kittl.auth.exchangeCode\n\
  \    purpose: Exchange the authorization code for the provider's token response payload.\n  - method: kittl.auth.getAuthToken\n    purpose: Restore a previously stored token on app reload.\n  - method: kittl.auth.getUserToken\n    purpose: Obtain the short-lived Kittl user JWT for app-backend verification.\nauthorization_model:\n  type: sdk-scopes\n  artifact: scopes/kittl-scopes.yml\n  description: >-\n    Beyond authentication, SDK call authorization is governed by the static scope set an\n    app declares in manifest.json config.scopes, enforced by the editor host at call time.\nsecurity_contact: security@kittl.com\nrelated:\n- scopes/kittl-scopes.yml\n- conventions/kittl-conventions.yml\n- json-schema/kittl-extension-manifest-schema.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kittl/refs/heads/main/authentication/kittl-authentication.yml
summary_line: jwt/oauth2-client/interactive-device-login · 3 schemes
tags:
- Company
- Design
- Graphic Design
- Creative Tools
- SDK
- Developer Platform
- Extensions
- Print On Demand
- E-Commerce
- AI
- Mockups
- Typography
---
