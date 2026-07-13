---
api_key_in: []
api_specs:
- filename: soundcloud-openapi.yml
  format: yaml
  label: SoundCloud API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcloud/refs/heads/main/openapi/soundcloud-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Soundcloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: SoundCloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: SoundCloud
provider_slug: soundcloud
scheme_count: 1
schemes:
- description: 'OAuth 2.1 with PKCE. Access tokens are short-lived (~1 hour). Use

    Authorization: OAuth {ACCESS_TOKEN} on each request.'
  flows:
  - authorizationUrl: https://secure.soundcloud.com/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://secure.soundcloud.com/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://secure.soundcloud.com/oauth/token
  name: oauth2
  sources:
  - openapi/soundcloud-openapi.yml
  type: oauth2
slug: soundcloud-authentication
source_filename: soundcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soundcloud-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.soundcloud.com/authorize\n    tokenUrl: https://secure.soundcloud.com/oauth/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://secure.soundcloud.com/oauth/token\n    scopes: 0\n  description: |-\n    OAuth 2.1 with PKCE. Access tokens are short-lived (~1 hour). Use\n    Authorization: OAuth {ACCESS_TOKEN} on each request.\n  sources:\n  - openapi/soundcloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundcloud/refs/heads/main/authentication/soundcloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Music
- Streaming
- Audio
- OAuth
- Tracks
- Playlists
---
