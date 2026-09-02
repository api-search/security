---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Elk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elk declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Elk
provider_slug: elk
scheme_count: 0
schemes: []
slug: elk-authentication
source_filename: elk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: derived\nsource: >-\n  Derived from Elk's own published MIT-licensed server source —\n  https://github.com/elk-zone/elk/blob/main/server/api/[server]/login.ts and\n  https://github.com/elk-zone/elk/blob/main/server/api/[server]/oauth/[origin].ts —\n  plus a live unauthenticated probe of https://elk.zone/api/list-servers on 2026-08-27.\n  Elk publishes no OpenAPI, so derive-authentication.py produced no profile (0 auth\n  profiles); this file was written by reading the deployed handlers instead.\nprovider: Elk\nproviderId: elk\napi: Elk Client API\nbaseURL: https://elk.zone/api\nsummary: >-\n  Elk has no API keys, no accounts of its own, and no credential it issues. It is an\n  OAuth 2.0 CLIENT and a broker: it holds a per-instance OAuth application registration\n  for each Mastodon server a user signs into, sends the user to that server's own\n  /oauth/authorize screen, and exchanges the returned authorization code for an access\n  token at\
  \ that server's /oauth/token. The bearer token that results belongs to the\n  Mastodon server, not to Elk. Nothing an integrator can obtain from Elk grants access\n  to anything.\nsecuritySchemes:\n  - name: none\n    type: none\n    applies_to:\n      - GET /api/list-servers\n    description: >-\n      Unauthenticated. Verified live 2026-08-27: HTTP 200, application/json, with\n      access-control-allow-origin \"*\" — a public, CORS-open list of the Mastodon server\n      domains Elk offers in its sign-in picker.\n  - name: mastodon_oauth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://{server}/oauth/authorize\n    tokenUrl: https://{server}/oauth/token\n    grant_type: authorization_code\n    response_type: code\n    scopes:\n      - read\n      - write\n      - follow\n      - push\n    applies_to:\n      - POST /api/{server}/login\n      - GET /api/{server}/oauth/{origin}\n    description: >-\n      Standard RFC 6749 authorization-code flow, but the\
  \ authorization server is chosen\n      at runtime by the end user — {server} is whatever Mastodon-compatible host they\n      typed. Elk registers an OAuth application per (origin, server) pair and caches\n      client_id/client_secret/vapid_key server-side; the client_secret never reaches the\n      browser. On success the handler 302-redirects to /signin/callback carrying the\n      access token in the query string.\n    x-notes:\n      - >-\n        Client credentials are per-deployment. A self-hosted Elk registers its own\n        applications against each Mastodon server; there is no shared Elk client_id.\n      - >-\n        The handler recovers from an invalid_client error (the Mastodon-side OAuth app\n        having been deleted) by invalidating its cached registration and retrying once.\n  - name: admin_key\n    type: apiKey\n    in: query\n    parameter: key\n    applies_to:\n      - GET /api/{server}/clear\n    description: >-\n      A single shared operator secret (Nuxt runtimeConfig.adminKey)\
  \ that authorises\n      deletion of a cached OAuth app registration. It is an operations control for\n      whoever runs the deployment, not a consumer credential — it is not issued, not\n      documented, and not obtainable. Compared with String equality; a wrong or missing\n      key returns HTTP 200 with {\"status\": false, \"error\": \"incorrect key\"} rather than\n      a 401/403.\ntoken_handling:\n  storage: >-\n    Access tokens are held client-side in browser storage by the Elk application (see\n    app/composables/users.ts). Elk operates no user database.\n  transport: Query string on the /signin/callback redirect, then Authorization bearer to the Mastodon server.\n  revocation: >-\n    At the Mastodon server, not at Elk. A user revokes Elk under their own instance's\n    authorised-applications settings.\ngaps:\n  - No published authentication documentation on docs.elk.zone; this profile is derived from source.\n  - No OpenAPI securitySchemes block exists to derive from.\n \
  \ - No /.well-known/oauth-authorization-server or oauth-protected-resource on elk.zone (both 404, 2026-08-27).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elk/refs/heads/main/authentication/elk-authentication.yml
summary_line: 0 schemes
tags:
- Fediverse
- Mastodon
- Open-Source
- Social Networking
- Social-Media
- Web-Client
- Progressive Web App
- Authentication
---
