---
api_key_in:
- query
- body
api_specs:
- filename: kongregate-server-api-openapi-original.json
  format: json
  label: Kongregate Server-Side API
  slug: kongregate-server-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-server-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kongregate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kongregate secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kongregate
provider_slug: kongregate
scheme_count: 3
schemes:
- description: Per-game private API key that identifies and authenticates the game server. Retrieved from the game's own /api page on Kongregate (https://www.kongregate.com/games/{username}/{game}/api).
  in: query
  name: api_key
  parameter_name: api_key
  scope: game
  secret: true
  sources:
  - openapi/kongregate-server-api-openapi-original.json
  type: apiKey
  used_by_operations:
  - server-api-authenticate
  - server-api-item-list
  - server-api-user-items
- description: The same private game API key, supplied in the JSON request body on POST operations.
  in: body
  name: api_key
  parameter_name: api_key
  scope: game
  secret: true
  sources:
  - openapi/kongregate-server-api-openapi-original.json
  type: apiKey
  used_by_operations:
  - server-api-characters
  - server-api-create-guild
  - server-api-destroy-guild
  - server-api-use-item
  - server-api-create-shared-link
  - server-api-destroy-shared-link
  - server-api-statistics
- description: Per-user, per-game authentication token that proves a specific player's identity. It is obtained CLIENT-side via the JavaScript API call kongregate.services.getGameAuthToken() and then passed to the game's own server, which exchanges it at GET /authenticate.json for the player's user_id and username.
  in: body
  name: game_auth_token
  parameter_name: game_auth_token
  rotation: Not stable. The documentation warns the token changes any time the user changes their password, so it must never be cached as a permanent identifier.
  scope: user
  secret: true
  sources:
  - openapi/kongregate-server-api-openapi-original.json
  type: apiKey
  used_by_operations:
  - server-api-authenticate
  - server-api-use-item
  - server-api-create-shared-link
  - server-api-destroy-shared-link
slug: kongregate-authentication
source_filename: kongregate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kongregate-server-api-openapi-original.json\ndocs: https://docs.kongregate.com/docs/concepts-authentication\nnote: >-\n  The published OpenAPI declares an EMPTY components.securitySchemes object and a\n  security: [{}] requirement, so a mechanical derive from the spec yields nothing. The\n  authentication model below is captured from the Kongregate developer documentation and\n  from the api_key / game_auth_token parameters that appear on the operations themselves.\n  This is a real contract-quality gap worth reporting to the provider: the credentials are\n  modelled as ordinary query/body parameters rather than as securitySchemes.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - body\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter_name: api_key\n  description: >-\n    Per-game private API key that identifies\
  \ and authenticates the game server. Retrieved\n    from the game's own /api page on Kongregate (https://www.kongregate.com/games/{username}/{game}/api).\n  scope: game\n  secret: true\n  sources:\n  - openapi/kongregate-server-api-openapi-original.json\n  used_by_operations:\n  - server-api-authenticate\n  - server-api-item-list\n  - server-api-user-items\n- name: api_key\n  type: apiKey\n  in: body\n  parameter_name: api_key\n  description: >-\n    The same private game API key, supplied in the JSON request body on POST operations.\n  scope: game\n  secret: true\n  sources:\n  - openapi/kongregate-server-api-openapi-original.json\n  used_by_operations:\n  - server-api-characters\n  - server-api-create-guild\n  - server-api-destroy-guild\n  - server-api-use-item\n  - server-api-create-shared-link\n  - server-api-destroy-shared-link\n  - server-api-statistics\n- name: game_auth_token\n  type: apiKey\n  in: body\n  parameter_name: game_auth_token\n  description: >-\n    Per-user, per-game\
  \ authentication token that proves a specific player's identity. It is\n    obtained CLIENT-side via the JavaScript API call kongregate.services.getGameAuthToken()\n    and then passed to the game's own server, which exchanges it at\n    GET /authenticate.json for the player's user_id and username.\n  scope: user\n  secret: true\n  rotation: >-\n    Not stable. The documentation warns the token changes any time the user changes their\n    password, so it must never be cached as a permanent identifier.\n  sources:\n  - openapi/kongregate-server-api-openapi-original.json\n  used_by_operations:\n  - server-api-authenticate\n  - server-api-use-item\n  - server-api-create-shared-link\n  - server-api-destroy-shared-link\nmodel:\n  style: two-credential (game secret + per-user token)\n  description: >-\n    Kongregate splits authentication across a client-side and a server-side half. The game\n    client asks the Kongregate JavaScript API for a game_auth_token scoped to that player and\n    that\
  \ game. The game's own backend then calls GET /authenticate.json with\n    api_key + user_id + game_auth_token, and Kongregate returns the authoritative username and\n    user_id. The api_key is a server-only secret.\n  stable_identifier: user_id\n  unstable_identifier: username\n  identifier_note: >-\n    A player's username can change over time; the user_id is constant. The documentation is\n    explicit that a game's database must key off user_id, never username.\ncallback_verification:\n  mechanism: signed request (HMAC-SHA256)\n  docs: https://docs.kongregate.com/docs/concepts-signed-requests\n  description: >-\n    Kongregate's outbound API callbacks are delivered as a signed_request POST parameter in the\n    Facebook signed-request format: a base64url HMAC-SHA256 signature and a base64url-encoded\n    JSON payload joined by a period. The receiver splits on the period, base64url-decodes and\n    JSON-parses the payload, asserts payload.algorithm == \"HMAC-SHA256\", then recomputes\n\
  \    HMAC-SHA256 over the encoded payload using the game's API key as the secret and compares.\n  parameter: signed_request\n  algorithm: HMAC-SHA256\n  secret: the game's private API key\nwarnings:\n- >-\n  The API key must never be used from the game client. The documentation notes that a CORS\n  error when calling a server API from the browser almost always means the API key has already\n  been exposed in client code.\n- >-\n  There is no OAuth 2.0, OpenID Connect, or mutual TLS surface. There are no scopes and no\n  granular permissions; the game API key is all-or-nothing for that game.\n- >-\n  Credentials travel as query-string parameters on GET operations, so they can appear in\n  intermediary and server access logs.\nrelated:\n- conventions/kongregate-conventions.yml\n- errors/kongregate-problem-types.yml\n- security/kongregate-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/authentication/kongregate-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Gaming
- Games
- Game Development
- Browser Games
- Virtual Goods
- Microtransactions
- Leaderboards
- Player Identity
- Unity
- Developer Platform
---
