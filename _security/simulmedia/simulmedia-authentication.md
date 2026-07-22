---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Simulmedia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Simulmedia secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Simulmedia
provider_slug: simulmedia
scheme_count: 2
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - DevGameServer/cmd/gameserver/gameserver.go
  token_request:
    content_type: application/x-www-form-urlencoded
    parameters:
    - name: client_id
      required: true
    - name: client_secret
      required: true
    - name: grant_type
      required: true
      value: client_credentials
    - description: PlayerWON game title id.
      name: tid
      required: true
    - description: Optional device advertising identifier appended to the token request.
      name: idfa
      required: false
  token_response:
    fields:
    - access_token
    - token_type
    - expires_in
  token_url: https://game.simulmedia-apis.com/token
  type: oauth2
- description: 'Access token returned by /token is sent as `Authorization: Bearer <token>` on the /session, /opportunity, /start, /progress, /complete and /abort calls.'
  name: BearerToken
  scheme: bearer
  sources:
  - UnitySDK/Assets/PlayerWon-SDK/Classes/Bridge.cs
  type: http
slug: simulmedia-authentication
source_filename: simulmedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/simulmedia/playerwon-sdk\ndocs: https://github.com/simulmedia/playerwon-sdk\napi: PlayerWON API\nbase_url: https://game.simulmedia-apis.com\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_delivery: bearer\n  notes: >-\n    The PlayerWON API uses OAuth 2.0 client-credentials. A game server exchanges\n    its CLIENT_ID / CLIENT_SECRET (plus the game title id, `tid`) at the /token\n    endpoint for a short-lived access token, then passes it to the game client\n    which sends it as an `Authorization: Bearer <token>` header on every\n    subsequent call. Secrets never ship in the game client.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://game.simulmedia-apis.com/token\n    token_request:\n      content_type: application/x-www-form-urlencoded\n      parameters:\n        - name: client_id\n          required: true\n\
  \        - name: client_secret\n          required: true\n        - name: grant_type\n          required: true\n          value: client_credentials\n        - name: tid\n          required: true\n          description: PlayerWON game title id.\n        - name: idfa\n          required: false\n          description: Optional device advertising identifier appended to the token request.\n    token_response:\n      fields: [access_token, token_type, expires_in]\n    sources: [DevGameServer/cmd/gameserver/gameserver.go]\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    description: >-\n      Access token returned by /token is sent as `Authorization: Bearer <token>`\n      on the /session, /opportunity, /start, /progress, /complete and /abort calls.\n    sources: [UnitySDK/Assets/PlayerWon-SDK/Classes/Bridge.cs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simulmedia/refs/heads/main/authentication/simulmedia-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Advertising
- Television
- Connected TV
- Games
- AdTech
- Rewarded Video
- Media Buying
---
