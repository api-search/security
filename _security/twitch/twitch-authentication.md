---
api_key_in: []
api_specs:
- filename: reference
  format: yaml
  label: Twitch API
  slug: twitch-api
  spec_type: OpenAPI
  url: https://dev.twitch.tv/docs/api/reference
- filename: twitch-eventsub-asyncapi.yml
  format: yaml
  label: Twitch EventSub
  slug: twitch-eventsub
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/asyncapi/twitch-eventsub-asyncapi.yml
- filename: twitch-extensions-openapi.yml
  format: yaml
  label: Twitch Extensions API
  slug: twitch-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-extensions-openapi.yml
- filename: twitch-drops-openapi.yml
  format: yaml
  label: Twitch Drops API
  slug: twitch-drops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-drops-openapi.yml
- filename: twitch-video-broadcast-openapi.yml
  format: yaml
  label: Twitch Video Broadcast API
  slug: twitch-video-broadcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-video-broadcast-openapi.yml
- filename: twitch-insights-analytics-openapi.yml
  format: yaml
  label: Twitch Insights and Analytics API
  slug: twitch-insights-and-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-insights-analytics-openapi.yml
- filename: twitch-igdb-openapi.yml
  format: yaml
  label: IGDB API
  slug: igdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-igdb-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Twitch Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Twitch secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Twitch
provider_slug: twitch
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  sources:
  - openapi/twitch-drops-openapi.yml
  - openapi/twitch-igdb-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://id.twitch.tv/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  sources:
  - openapi/twitch-extensions-openapi.yml
  - openapi/twitch-helix-openapi.yml
  - openapi/twitch-insights-analytics-openapi.yml
  type: oauth2
- description: App Access Token obtained via Client Credentials grant
  name: appAccessToken
  scheme: bearer
  sources:
  - openapi/twitch-helix-openapi.yml
  type: http
slug: twitch-authentication
source_filename: twitch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/twitch-drops-openapi.yml, openapi/twitch-extensions-openapi.yml, openapi/twitch-helix-openapi.yml,\n  openapi/twitch-igdb-openapi.yml, openapi/twitch-insights-analytics-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.twitch.tv/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/twitch-drops-openapi.yml\n  - openapi/twitch-igdb-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.twitch.tv/oauth2/authorize\n    tokenUrl: https://id.twitch.tv/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/twitch-extensions-openapi.yml\n  - openapi/twitch-helix-openapi.yml\n  - openapi/twitch-insights-analytics-openapi.yml\n- name: appAccessToken\n  type: http\n  scheme: bearer\n  description:\
  \ App Access Token obtained via Client Credentials grant\n  sources:\n  - openapi/twitch-helix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/authentication/twitch-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
---
