---
api_key_in: []
auth_types:
- oauth2
description: 'The Sonos Control API authenticates third-party integrations with OAuth 2.0 (RFC 6749) using the authorization code grant. The integration redirects the user to the Sonos login service, receives an authorization code, then exchanges it for an access token and refresh token. Access tokens are sent as a Bearer token on every Control API request to api.ws.sonos.com. Confirmed live: the authorize and token endpoints return HTTP 400 to unparameterised requests (present), and api.ws.sonos.com/control/api/v1/households returns 401 without a token.'
kind: authentication
layout: security
method: searched
name: Sonos Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sonos secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sonos
provider_slug: sonos
scheme_count: 1
schemes:
- description: 'OAuth 2.0 authorization code grant. Single scope: playback-control-all. Access tokens are short-lived and refreshed with the refresh token via the token endpoint.'
  flows:
  - authorizationUrl: https://api.sonos.com/login/v3/oauth
    flow: authorizationCode
    refreshUrl: https://api.sonos.com/login/v3/oauth/access
    scopes:
    - description: Control access to a household's Sonos players and groups.
      scope: playback-control-all
    tokenUrl: https://api.sonos.com/login/v3/oauth/access
  name: SonosOAuth
  sources:
  - https://docs.sonos.com/docs/authorize
  - https://docs.sonos.com/reference/create-authorization-code
  - https://docs.sonos.com/reference/createtoken
  - https://docs.sonos.com/reference/refreshtoken
  type: oauth2
slug: sonos-authentication
source_filename: sonos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sonos.com/docs/authorize\ndescription: >-\n  The Sonos Control API authenticates third-party integrations with OAuth 2.0\n  (RFC 6749) using the authorization code grant. The integration redirects the\n  user to the Sonos login service, receives an authorization code, then\n  exchanges it for an access token and refresh token. Access tokens are sent as\n  a Bearer token on every Control API request to api.ws.sonos.com. Confirmed\n  live: the authorize and token endpoints return HTTP 400 to unparameterised\n  requests (present), and api.ws.sonos.com/control/api/v1/households returns 401\n  without a token.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  token_delivery: bearer-header\nschemes:\n- name: SonosOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization code grant. Single scope: playback-control-all.\n    Access tokens are short-lived and refreshed with the refresh\
  \ token via the\n    token endpoint.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.sonos.com/login/v3/oauth\n    tokenUrl: https://api.sonos.com/login/v3/oauth/access\n    refreshUrl: https://api.sonos.com/login/v3/oauth/access\n    scopes:\n    - scope: playback-control-all\n      description: Control access to a household's Sonos players and groups.\n  sources:\n  - https://docs.sonos.com/docs/authorize\n  - https://docs.sonos.com/reference/create-authorization-code\n  - https://docs.sonos.com/reference/createtoken\n  - https://docs.sonos.com/reference/refreshtoken\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonos/refs/heads/main/authentication/sonos-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Audio
- Music
- Smart Home
- IoT
- Streaming
- Speakers
- Home Automation
- Voice
---
