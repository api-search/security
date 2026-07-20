---
api_key_in: []
api_specs:
- filename: epidemic-sound-partner-content-api-openapi.yml
  format: yaml
  label: Epidemic Sound Partner Content API
  slug: epidemic-sound-partner-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epidemic-sound/refs/heads/main/openapi/epidemic-sound-partner-content-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Epidemic Sound Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Epidemic Sound secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Epidemic Sound
provider_slug: epidemic-sound
scheme_count: 3
schemes:
- description: 'API key authentication for server-to-server communication.

    Pass your API key as a Bearer token in the Authorization header.

    API keys are prefixed with `epidemic_live_`.


    > **Example Header:** `Authorization: Bearer [example key]`'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/epidemic-sound-partner-content-api-openapi.yml
  type: http
- description: 'Partner authentication is handled with short lived partner access tokens.

    Use your api credentials to request these tokens.

    The access token is of JWT format and should be passed in a header with your API requests:


    > **Example Header:** `Authorization: Bearer [example key]`'
  name: PartnerAuth
  scheme: Bearer
  sources:
  - openapi/epidemic-sound-partner-content-api-openapi.yml
  type: http
- description: 'For users signing in with an Epidemic Sound account, user authentication is

    handled with OpenID Connect, which is a layer on top of OAuth 2.0.


    > **Example Header:** `Authorization: Bearer [example key]`'
  flows:
  - authorizationUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/token
  name: EpidemicSoundConnectAuth
  sources:
  - openapi/epidemic-sound-partner-content-api-openapi.yml
  type: oauth2
slug: epidemic-sound-authentication
source_filename: epidemic-sound-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epidemic-sound-partner-content-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API key authentication for server-to-server communication.\n    Pass your API key as a Bearer token in the Authorization header.\n    API keys are prefixed with `epidemic_live_`.\n\n    > **Example Header:** `Authorization: Bearer [example key]`\n  sources:\n  - openapi/epidemic-sound-partner-content-api-openapi.yml\n- name: PartnerAuth\n  type: http\n  scheme: Bearer\n  description: |-\n    Partner authentication is handled with short lived partner access tokens.\n    Use your api credentials to request these tokens.\n    The access token is of JWT format and should be passed in a header with your API requests:\n\n    > **Example Header:** `Authorization: Bearer [example key]`\n  sources:\n  - openapi/epidemic-sound-partner-content-api-openapi.yml\n\
  - name: EpidemicSoundConnectAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/auth\n    tokenUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/token\n    scopes: 0\n  description: |-\n    For users signing in with an Epidemic Sound account, user authentication is\n    handled with OpenID Connect, which is a layer on top of OAuth 2.0.\n\n    > **Example Header:** `Authorization: Bearer [example key]`\n  sources:\n  - openapi/epidemic-sound-partner-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epidemic-sound/refs/heads/main/authentication/epidemic-sound-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Music
- Sound Effects
- Royalty-Free Music
- Audio
- Audio Licensing
- Soundtracking
- Sync Licensing
- Creators
- Video
- AI Voiceover
- Semantic Search
- MCP
---
