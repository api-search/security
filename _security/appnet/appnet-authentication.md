---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Appnet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
overview: App.net secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and clientCredentials flow(s).
provider_name: App.net
provider_slug: appnet
scheme_count: 1
schemes:
- description: 'App.net authenticates with OAuth 2.0 bearer access tokens. Two token classes exist: user tokens (act on behalf of a specific user) and app tokens (client-credentials, act on behalf of the application). Tokens may be passed via the Authorization: Bearer header (preferred), an access_token query-string parameter, or an access_token body field on PUT/POST/PATCH.'
  flows:
  - authorizationUrl: https://account.app.net/oauth/authenticate
    flow: authorizationCode
    forceDialogUrl: https://account.app.net/oauth/authorize
    label: Web flow (server-side)
    tokenUrl: https://account.app.net/oauth/access_token
  - authorizationUrl: https://account.app.net/oauth/authenticate
    flow: implicit
    label: Web flow (client-side)
  - flow: clientCredentials
    label: App access token flow
    tokenUrl: https://account.app.net/oauth/access_token
  - flow: password
    label: Password flow (restricted; requires special permission)
    tokenUrl: https://account.app.net/oauth/access_token
  name: OAuth2
  scope_header: X-OAuth-Scopes
  scopes_ref: scopes/appnet-scopes.yml
  type: oauth2
slug: appnet-authentication
source_filename: appnet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/appdotnet/api-spec/blob/new-docs/content/reference/authentication/index.md\ndocs: https://github.com/appdotnet/api-spec/tree/new-docs/content/reference/authentication\nnote: >-\n  App.net is retired (shut down 2017-03-14); the authorization/token hosts under\n  account.app.net no longer resolve. This profile is transcribed verbatim from the\n  preserved api-spec authentication documentation.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - password\n  - clientCredentials\n  token_style: bearer\n  transport: HTTPS required for all requests\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    App.net authenticates with OAuth 2.0 bearer access tokens. Two token classes exist:\n    user tokens (act on behalf of a specific user) and app tokens (client-credentials,\n    act on behalf of the application). Tokens may be passed via the Authorization: Bearer\n\
  \    header (preferred), an access_token query-string parameter, or an access_token body\n    field on PUT/POST/PATCH.\n  flows:\n  - flow: authorizationCode\n    label: Web flow (server-side)\n    authorizationUrl: https://account.app.net/oauth/authenticate\n    forceDialogUrl: https://account.app.net/oauth/authorize\n    tokenUrl: https://account.app.net/oauth/access_token\n  - flow: implicit\n    label: Web flow (client-side)\n    authorizationUrl: https://account.app.net/oauth/authenticate\n  - flow: clientCredentials\n    label: App access token flow\n    tokenUrl: https://account.app.net/oauth/access_token\n  - flow: password\n    label: Password flow (restricted; requires special permission)\n    tokenUrl: https://account.app.net/oauth/access_token\n  scope_header: X-OAuth-Scopes\n  scopes_ref: scopes/appnet-scopes.yml\ntoken_kinds:\n- kind: user\n  description: Represents access to API resources on behalf of a specific user.\n- kind: app\n  description: >-\n    Client-credentials\
  \ token representing the application itself; only developer-account\n    apps can request tokens for other users.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appnet/refs/heads/main/authentication/appnet-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Social
- Microblogging
- Messaging
- Real Time
- Streaming
- Developer Platform
- OAuth
- Defunct
---
