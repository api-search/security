---
api_key_in:
- header
- query
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Groupme Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: GroupMe secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: GroupMe
provider_slug: groupme
scheme_count: 3
schemes:
- in: header
  name: AccessTokenHeader
  parameter_name: X-Access-Token
  recommended: true
  sources:
  - https://dev.groupme.com/docs/v3
  type: apiKey
- in: query
  name: AccessTokenQuery
  note: Accepted but discouraged by the docs (never put the token in the URL).
  parameter_name: token
  recommended: false
  sources:
  - https://dev.groupme.com/docs/v3
  type: apiKey
- authorizationUrl: https://oauth.groupme.com/oauth/authorize
  flow: implicit
  name: OAuth2
  note: Token-grant OAuth. The application key is issued when registering an app at dev.groupme.com; the user is redirected to the authorize URL and an access_token is returned to the registered callback. No scope system.
  scopes: {}
  sources:
  - https://dev.groupme.com/tutorials/oauth
  type: oauth2
slug: groupme-authentication
source_filename: groupme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.groupme.com/docs/v3\ndocs: https://dev.groupme.com/tutorials/oauth\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [implicit]\nnotes: >-\n  GroupMe API v3 authenticates every request with a per-user access token. The\n  documentation directs developers to always send the token in the\n  X-Access-Token header and never in the URL query string, though the query\n  parameter token= is also historically accepted. Tokens are obtained either\n  from the developer's own access-token page (dev.groupme.com) or via the OAuth\n  flow for third-party applications. GroupMe's OAuth is a simplified\n  token-grant: an application redirects the user to the authorize endpoint and\n  receives an access token back on the callback (no scopes, no refresh token,\n  no OIDC discovery). Push (Faye/Bayeux) and bot callbacks reuse the same\n  access token, passed in the Bayeux ext field for push subscriptions.\n\
  schemes:\n  - name: AccessTokenHeader\n    type: apiKey\n    in: header\n    parameter_name: X-Access-Token\n    recommended: true\n    sources: [https://dev.groupme.com/docs/v3]\n  - name: AccessTokenQuery\n    type: apiKey\n    in: query\n    parameter_name: token\n    recommended: false\n    note: Accepted but discouraged by the docs (never put the token in the URL).\n    sources: [https://dev.groupme.com/docs/v3]\n  - name: OAuth2\n    type: oauth2\n    flow: implicit\n    authorizationUrl: https://oauth.groupme.com/oauth/authorize\n    scopes: {}\n    note: >-\n      Token-grant OAuth. The application key is issued when registering an app\n      at dev.groupme.com; the user is redirected to the authorize URL and an\n      access_token is returned to the registered callback. No scope system.\n    sources: [https://dev.groupme.com/tutorials/oauth]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupme/refs/heads/main/authentication/groupme-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Consumer
- Messaging
- Chat
- Bots
- Group Messaging
- Communication
- Social
---
