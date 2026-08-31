---
api_key_in: []
api_specs:
- filename: lvt-cameras-api-openapi.yml
  format: yaml
  label: LVT Cameras API
  slug: lvt-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-cameras-api-openapi.yml
- filename: lvt-events-api-openapi.yml
  format: yaml
  label: LVT Events API
  slug: lvt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-events-api-openapi.yml
- filename: lvt-liveunits-api-openapi.yml
  format: yaml
  label: LVT Live Units API
  slug: lvt-liveunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-liveunits-api-openapi.yml
- filename: lvt-locations-api-openapi.yml
  format: yaml
  label: LVT Locations API
  slug: lvt-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-locations-api-openapi.yml
- filename: lvt-media-api-openapi.yml
  format: yaml
  label: LVT Media API
  slug: lvt-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-media-api-openapi.yml
- filename: lvt-publickeys-api-openapi.yml
  format: yaml
  label: LVT Public Keys API
  slug: lvt-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-publickeys-api-openapi.yml
- filename: lvt-streams-api-openapi.yml
  format: yaml
  label: LVT Streams API
  slug: lvt-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-streams-api-openapi.yml
- filename: lvt-talkdown-api-openapi.yml
  format: yaml
  label: LVT Talkdown API
  slug: lvt-talkdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-talkdown-api-openapi.yml
- filename: lvt-webhooks-api-openapi.yml
  format: yaml
  label: LVT Webhooks API
  slug: lvt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lvt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LVT secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LVT
provider_slug: lvt
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.lvt.com/oauth2/v1/token
  name: OAuth2
  sources:
  - openapi/lvt-partner-api-openapi.yml
  type: oauth2
slug: lvt-authentication
source_filename: lvt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/lvt-partner-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.lvt.com/oauth2/v1/token\n    scopes: 3\n  sources:\n  - openapi/lvt-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/authentication/lvt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Physical Security
- Video Surveillance
- Camera
- Video Streaming
- WebRTC
- RTSP
- ONVIF
- IoT
- Alerts
- Webhook
- Public Safety
- Retail
- Critical Infrastructure
---
