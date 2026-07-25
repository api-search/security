---
api_key_in: []
api_specs:
- filename: rockbot-audio-messaging-api-openapi.yml
  format: yaml
  label: Rockbot Audio Messaging API
  slug: rockbot-audio-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-audio-messaging-api-openapi.yml
- filename: rockbot-auth-api-openapi.yml
  format: yaml
  label: Rockbot Auth API
  slug: rockbot-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-auth-api-openapi.yml
- filename: rockbot-data-api-openapi.yml
  format: yaml
  label: Rockbot Data API
  slug: rockbot-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-data-api-openapi.yml
- filename: rockbot-devices-api-openapi.yml
  format: yaml
  label: Rockbot Devices API
  slug: rockbot-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-devices-api-openapi.yml
- filename: rockbot-music-api-openapi.yml
  format: yaml
  label: Rockbot Music API
  slug: rockbot-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-music-api-openapi.yml
- filename: rockbot-signage-api-openapi.yml
  format: yaml
  label: Rockbot Signage API
  slug: rockbot-signage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-signage-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Rockbot Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Rockbot secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Rockbot
provider_slug: rockbot
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.rockbot.com/v5/api-clients/token
  name: oauth2
  sources:
  - openapi/rockbot-openapi.yml
  type: oauth2
slug: rockbot-authentication
source_filename: rockbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rockbot-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.rockbot.com/v5/api-clients/token\n    scopes: 0\n  description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued\n    by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it\n    as `Authorization: Bearer ACCESS_TOKEN`.'\n  sources:\n  - openapi/rockbot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/authentication/rockbot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Music
- Digital Signage
- Audio Messaging
- Retail Media
- In-Location Media
- Media
- Entertainment
---
