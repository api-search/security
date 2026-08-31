---
api_key_in:
- header
- query
api_specs:
- filename: zype-platform.json
  format: json
  label: Zype Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-platform.json
- filename: zype-playout-scheduler.json
  format: json
  label: Zype Playout Scheduler API
  slug: playout-scheduler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-playout-scheduler.json
- filename: zype-monetization.json
  format: json
  label: Zype Monetization API
  slug: monetization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-monetization.json
- filename: zype-consumers.json
  format: json
  label: Zype Consumers API
  slug: consumers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-consumers.json
- filename: zype-live-3.json
  format: json
  label: Zype Live API (V3)
  slug: live-3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-live-3.json
- filename: zype-zobjects.json
  format: json
  label: Zype Zobjects API
  slug: zobjects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-zobjects.json
- filename: zype-analytics-v3.json
  format: json
  label: Zype Analytics API (V3)
  slug: analytics-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-analytics-v3.json
- filename: zype-analytics.json
  format: json
  label: Zype Analytics API (V2)
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-analytics.json
- filename: zype-content-regions.json
  format: json
  label: Zype Custom Regions API
  slug: content-regions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-regions.json
- filename: zype-content-rule-groups.json
  format: json
  label: Zype Content Rule Groups API
  slug: content-rule-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-rule-groups.json
- filename: zype-content-rules.json
  format: json
  label: Zype Content Rule Profiles API
  slug: content-rules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-rules.json
- filename: zype-tve.json
  format: json
  label: Zype TVE API
  slug: tve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-tve.json
- filename: zype-login.json
  format: json
  label: Zype Consumer Authentication API
  slug: login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-login.json
- filename: zype-player.json
  format: json
  label: Zype Player API
  slug: player
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-player.json
- filename: zype-uploads.json
  format: json
  label: Zype Uploads API
  slug: uploads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-uploads.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zype Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zype secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zype
provider_slug: zype
scheme_count: 3
schemes:
- in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/zype-analytics-v3.json
  - openapi/zype-analytics.json
  - openapi/zype-consumers.json
  - openapi/zype-content-regions.json
  - openapi/zype-content-rule-groups.json
  - openapi/zype-content-rules.json
  - openapi/zype-live-3.json
  - openapi/zype-monetization.json
  - openapi/zype-platform.json
  - openapi/zype-player.json
  - openapi/zype-tve.json
  - openapi/zype-uploads.json
  - openapi/zype-zobjects.json
  type: apiKey
- bearerFormat: OAuth access token
  description: OAuth access token of the consumer
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zype-analytics-v3.json
  - openapi/zype-analytics.json
  - openapi/zype-consumers.json
  - openapi/zype-content-regions.json
  - openapi/zype-content-rule-groups.json
  - openapi/zype-content-rules.json
  - openapi/zype-live-3.json
  - openapi/zype-monetization.json
  - openapi/zype-platform.json
  - openapi/zype-player.json
  - openapi/zype-uploads.json
  - openapi/zype-zobjects.json
  type: http
- in: header
  name: api_key
  parameter: X-API-Key
  sources:
  - openapi/zype-playout-scheduler.json
  type: apiKey
slug: zype-authentication
source_filename: zype-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: derived\nsource: openapi/zype-analytics-v3.json, openapi/zype-analytics.json, openapi/zype-consumers.json,\n  openapi/zype-content-regions.json, openapi/zype-content-rule-groups.json, openapi/zype-content-rules.json,\n  openapi/zype-live-3.json, openapi/zype-monetization.json, openapi/zype-platform.json, openapi/zype-player.json,\n  openapi/zype-playout-scheduler.json, openapi/zype-tve.json ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/zype-analytics-v3.json\n  - openapi/zype-analytics.json\n  - openapi/zype-consumers.json\n  - openapi/zype-content-regions.json\n  - openapi/zype-content-rule-groups.json\n  - openapi/zype-content-rules.json\n  - openapi/zype-live-3.json\n  - openapi/zype-monetization.json\n  - openapi/zype-platform.json\n  - openapi/zype-player.json\n  - openapi/zype-tve.json\n  - openapi/zype-uploads.json\n\
  \  - openapi/zype-zobjects.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth access token\n  description: OAuth access token of the consumer\n  sources:\n  - openapi/zype-analytics-v3.json\n  - openapi/zype-analytics.json\n  - openapi/zype-consumers.json\n  - openapi/zype-content-regions.json\n  - openapi/zype-content-rule-groups.json\n  - openapi/zype-content-rules.json\n  - openapi/zype-live-3.json\n  - openapi/zype-monetization.json\n  - openapi/zype-platform.json\n  - openapi/zype-player.json\n  - openapi/zype-uploads.json\n  - openapi/zype-zobjects.json\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/zype-playout-scheduler.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/authentication/zype-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Video
- Streaming
- OTT
- Video CMS
- FAST
- Linear TV
- Playout
- Monetization
- Live Streaming
- Analytics
- Media & Entertainment
- DRM
- Advertising
- Encoding
- EPG
---
