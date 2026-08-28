---
api_key_in: []
api_specs:
- filename: lvt-partner-api-openapi.yml
  format: yaml
  label: LVT Partner API
  slug: lvt-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-partner-api-openapi.yml
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
- Cameras
- Video Streaming
- WebRTC
- RTSP
- ONVIF
- IoT
- Alerts
- Webhooks
- Public Safety
- Retail
- Critical Infrastructure
---
