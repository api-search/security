---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bitstrips Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bitstrips secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bitstrips
provider_slug: bitstrips
scheme_count: 2
schemes:
- description: OAuth2 authorization code flow with PKCE (S256). Authorization is initiated at www.bitmoji.com/connect; tokens are exchanged and refreshed at the Snap token endpoint.
  flows:
  - authorizationUrl: https://www.bitmoji.com/connect/
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://bitmoji.api.snapchat.com/direct/token
    revocationUrl: https://bitmoji.api.snapchat.com/direct/token/revoke
    scopes: {}
    tokenUrl: https://bitmoji.api.snapchat.com/direct/token
  name: BitmojiDirectOAuth2
  sources:
  - https://github.com/Bitmoji/BitmojiForDevelopers/blob/main/docs/DIRECT_AUTH_FOR_DEVELOPERS.md
  type: oauth2
- description: 'API requests to bitmoji.api.snapchat.com/direct authenticate with the OAuth2 access token as an HTTP bearer token (`Authorization: Bearer <access_token>`).'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://github.com/Bitmoji/BitmojiForDevelopers/blob/main/docs/DIRECT_AUTH_FOR_DEVELOPERS.md
  type: http
slug: bitstrips-authentication
source_filename: bitstrips-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/Bitmoji/BitmojiForDevelopers/blob/main/docs/DIRECT_AUTH_FOR_DEVELOPERS.md\ndocs: https://github.com/Bitmoji/BitmojiForDevelopers\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  pkce: required\n  bearer_tokens: true\nnotes: >-\n  Bitmoji Direct authorization is a standard OAuth2 authorization-code flow with\n  PKCE (S256) required. Apps must be registered in the Snap Kit Developer portal\n  (an Org and an App). Access tokens expire in 1 hour; refresh tokens expire in\n  90 days. API requests carry the token as `Authorization: Bearer <access_token>`.\n  Named OAuth scopes are not published in the developer docs; authorization grants\n  access to avatar data, sticker packs, and search. Snap has deprecated the\n  \"Bitmoji For Identity\" product.\nschemes:\n- name: BitmojiDirectOAuth2\n  type: oauth2\n  description: >-\n    OAuth2 authorization code flow with PKCE (S256).\
  \ Authorization is initiated\n    at www.bitmoji.com/connect; tokens are exchanged and refreshed at the Snap\n    token endpoint.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.bitmoji.com/connect/\n    tokenUrl: https://bitmoji.api.snapchat.com/direct/token\n    refreshUrl: https://bitmoji.api.snapchat.com/direct/token\n    revocationUrl: https://bitmoji.api.snapchat.com/direct/token/revoke\n    pkce: S256\n    scopes: {}\n  sources:\n  - https://github.com/Bitmoji/BitmojiForDevelopers/blob/main/docs/DIRECT_AUTH_FOR_DEVELOPERS.md\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API requests to bitmoji.api.snapchat.com/direct authenticate with the OAuth2\n    access token as an HTTP bearer token (`Authorization: Bearer <access_token>`).\n  sources:\n  - https://github.com/Bitmoji/BitmojiForDevelopers/blob/main/docs/DIRECT_AUTH_FOR_DEVELOPERS.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitstrips/refs/heads/main/authentication/bitstrips-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Consumer
- Avatars
- Stickers
- Bitmoji
- Messaging
- Images
- OAuth
- Social
---
