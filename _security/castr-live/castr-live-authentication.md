---
api_key_in:
- header
api_specs:
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Live Streams API
  slug: castr-live-live-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Sub-Second Streams API
  slug: castr-live-sub-second-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Video Hosting and VOD API
  slug: castr-live-video-hosting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Analytics and Activity API
  slug: castr-live-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Webhooks API
  slug: castr-live-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Castr Live Authentication
name_suffix: Authentication
oauth_flows: []
overview: Castr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Castr
provider_slug: castr-live
scheme_count: 1
schemes:
- description: API token issued from the Castr account settings API section (https://castr.com/app/manage/api), sent in the authorization header.
  in: header
  name: apiToken
  parameter: authorization
  sources:
  - openapi/castr-live-openapi.yml
  type: apiKey
slug: castr-live-authentication
source_filename: castr-live-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/castr-live-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: API token issued from the Castr account settings API section (https://castr.com/app/manage/api),\n    sent in the authorization header.\n  sources:\n  - openapi/castr-live-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/authentication/castr-live-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Live Streaming
- Multistreaming
- Video Hosting
- VOD
- Video
- Restreaming
- Sub-Second Streaming
- WebRTC
- Analytics
- Webhooks
---
