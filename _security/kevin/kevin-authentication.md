---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kevin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kevin. secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kevin.
provider_slug: kevin
scheme_count: 2
schemes:
- applies_to:
  - General-Service
  - Payment-Initiation-Service
  description: Client-level credentials (Client-Id + Client-Secret) identify the merchant / project. Used for General and Payment Initiation Service calls. In the SDK this is `new kevin.Client(clientId, clientSecret)`.
  in: header
  name: PlatformClientCredentials
  parameters:
  - Client-Id
  - Client-Secret
  type: apiKey
- applies_to:
  - Account-Information-Service
  description: 'Account Information Service uses a user-authorization flow: `startAuth` (with requested scopes + a Redirect-URL) returns an auth key; `receiveToken` exchanges the auth key for a bearer + refresh token pair; `refreshToken` exchanges a refresh token for a new bearer token; `receiveTokenContent` inspects a bearer token. Bearer tokens authorize per-account AIS calls.'
  flow: authorizationCode
  name: UserBearerToken
  operations:
  - startAuth
  - receiveToken
  - refreshToken
  - receiveTokenContent
  scheme: bearer
  scopes_ref: scopes/kevin-scopes.yml
  type: oauth2
slug: kevin-authentication
source_filename: kevin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.npmjs.com/package/@kevin.eu/kevin-platform-client (official SDK) + https://developer.kevin.eu/\ndocs: https://developer.kevin.eu/platform/general/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: PlatformClientCredentials\n  type: apiKey\n  in: header\n  description: >-\n    Client-level credentials (Client-Id + Client-Secret) identify the merchant /\n    project. Used for General and Payment Initiation Service calls. In the SDK\n    this is `new kevin.Client(clientId, clientSecret)`.\n  parameters:\n  - Client-Id\n  - Client-Secret\n  applies_to: [General-Service, Payment-Initiation-Service]\n- name: UserBearerToken\n  type: oauth2\n  scheme: bearer\n  description: >-\n    Account Information Service uses a user-authorization flow: `startAuth` (with\n    requested scopes + a Redirect-URL) returns an auth key; `receiveToken`\n    exchanges\
  \ the auth key for a bearer + refresh token pair; `refreshToken`\n    exchanges a refresh token for a new bearer token; `receiveTokenContent`\n    inspects a bearer token. Bearer tokens authorize per-account AIS calls.\n  flow: authorizationCode\n  operations: [startAuth, receiveToken, refreshToken, receiveTokenContent]\n  applies_to: [Account-Information-Service]\n  scopes_ref: scopes/kevin-scopes.yml\nnotes: >-\n  A2A open-banking (PSD2) provider. Merchant/project auth is header client\n  credentials; end-user account access is a scoped, redirect-based token flow.\n  No mutualTLS / mTLS scheme was documented in the public SDK. Derived from the\n  official Node SDK and archived developer reference; live docs host\n  (developer.kevin.eu) no longer resolves as of 2026-07.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevin/refs/heads/main/authentication/kevin-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Payments
- Open Banking
- Account to Account
- PSD2
- Fintech
- Bank Payments
- Payment Initiation
- Account Information
- Europe
---
