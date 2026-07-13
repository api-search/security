---
api_key_in:
- query
api_specs:
- filename: zoom-chat--openapi-original.yml
  format: yaml
  label: Zoom Chat API
  slug: zoom-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-chat--openapi-original.yml
- filename: zoom-group--openapi-original.yml
  format: yaml
  label: Zoom Group API
  slug: zoom-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-group--openapi-original.yml
- filename: zoom-device--openapi-original.yml
  format: yaml
  label: Zoom Device API
  slug: zoom-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-device--openapi-original.yml
- filename: zoom-im--openapi-original.yml
  format: yaml
  label: Zoom Instant Message API
  slug: zoom-instant-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-im--openapi-original.yml
- filename: zoom-account--openapi-original.yml
  format: yaml
  label: Zoom Account API
  slug: zoom-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-account--openapi-original.yml
- filename: zoom-recording--openapi-original.yml
  format: yaml
  label: Zoom Recording API
  slug: zoom-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-recording--openapi-original.yml
- filename: zoom-meeting--openapi-original.yml
  format: yaml
  label: Zoom Meeting API
  slug: zoom-meeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting--openapi-original.yml
- filename: zoom-metrics--openapi-original.yml
  format: yaml
  label: Zoom Metrics API
  slug: zoom-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-metrics--openapi-original.yml
- filename: zoom-report--openapi-original.yml
  format: yaml
  label: Zoom Report API
  slug: zoom-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-report--openapi-original.yml
- filename: zoom-user--openapi-original.yml
  format: yaml
  label: Zoom User API
  slug: zoom-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-user--openapi-original.yml
- filename: zoom-webinar--openapi-original.yml
  format: yaml
  label: Zoom Webinar API
  slug: zoom-webinar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-webinar--openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoom secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoom
provider_slug: zoom
scheme_count: 4
schemes:
- description: Zoom uses OAuth 2.0 for authentication. Server-to-Server OAuth and standard OAuth apps are supported.
  flows:
  - authorizationUrl: https://zoom.us/oauth/authorize
    flow: authorizationCode
    scopes: 19
    tokenUrl: https://zoom.us/oauth/token
  name: oauth2
  sources:
  - openapi/zoom-meeting-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: Bearer token obtained from OAuth 2.0 Server-to-Server or standard OAuth flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zoom-meeting-api-openapi.yml
  type: http
- in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/zoom-openapi-original.yml
  type: apiKey
- in: query
  name: api_secret
  parameter: api_secret
  sources:
  - openapi/zoom-openapi-original.yml
  type: apiKey
slug: zoom-authentication
source_filename: zoom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoom-meeting-api-openapi.yml, openapi/zoom-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://zoom.us/oauth/authorize\n    tokenUrl: https://zoom.us/oauth/token\n    scopes: 19\n  description: Zoom uses OAuth 2.0 for authentication. Server-to-Server OAuth and standard OAuth\n    apps are supported.\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from OAuth 2.0 Server-to-Server or standard OAuth flow.\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/zoom-openapi-original.yml\n- name: api_secret\n  type: apiKey\n\
  \  in: query\n  parameter: api_secret\n  sources:\n  - openapi/zoom-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/authentication/zoom-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
---
