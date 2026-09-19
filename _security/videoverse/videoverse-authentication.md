---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: videoverse-catch-me-up-api-openapi.yml
  format: yaml
  label: VideoVerse Catch me up API
  slug: videoverse-catch-me-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-catch-me-up-api-openapi.yml
- filename: videoverse-clips-api-openapi.yml
  format: yaml
  label: VideoVerse Clips API
  slug: videoverse-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-clips-api-openapi.yml
- filename: videoverse-content-api-openapi.yml
  format: yaml
  label: VideoVerse Content API
  slug: videoverse-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-content-api-openapi.yml
- filename: videoverse-entity-member-api-openapi.yml
  format: yaml
  label: VideoVerse Entity Member API
  slug: videoverse-entity-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-entity-member-api-openapi.yml
- filename: videoverse-highlight-clips-api-openapi.yml
  format: yaml
  label: VideoVerse Highlight Clips API
  slug: videoverse-highlight-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-highlight-clips-api-openapi.yml
- filename: videoverse-highlights-api-openapi.yml
  format: yaml
  label: VideoVerse Highlights API
  slug: videoverse-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-highlights-api-openapi.yml
- filename: videoverse-match-schedule-api-openapi.yml
  format: yaml
  label: VideoVerse Match Schedule API
  slug: videoverse-match-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-match-schedule-api-openapi.yml
- filename: videoverse-match-video-api-openapi.yml
  format: yaml
  label: VideoVerse Match Video API
  slug: videoverse-match-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-match-video-api-openapi.yml
- filename: videoverse-partner-api-openapi.yml
  format: yaml
  label: VideoVerse Partner API
  slug: videoverse-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-partner-api-openapi.yml
- filename: videoverse-player-api-openapi.yml
  format: yaml
  label: VideoVerse Player API
  slug: videoverse-player-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-player-api-openapi.yml
- filename: videoverse-streams-api-openapi.yml
  format: yaml
  label: VideoVerse Streams API
  slug: videoverse-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-streams-api-openapi.yml
- filename: videoverse-team-api-openapi.yml
  format: yaml
  label: VideoVerse Team API
  slug: videoverse-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-team-api-openapi.yml
- filename: videoverse-tournament-api-openapi.yml
  format: yaml
  label: VideoVerse Tournament API
  slug: videoverse-tournament-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-tournament-api-openapi.yml
- filename: videoverse-webhook-api-openapi.yml
  format: yaml
  label: VideoVerse Webhook API
  slug: videoverse-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Videoverse Authentication
name_suffix: Authentication
oauth_flows: []
overview: VideoVerse secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VideoVerse
provider_slug: videoverse
scheme_count: 2
schemes:
- description: 'Partner Access Key issued by Magnifi. Documented example prefix: pak_.'
  in: header
  name: AccessKey
  parameter: x-access-key
  sources:
  - openapi/videoverse-magnifi-partner-openapi.yml
  type: apiKey
- description: Partner Access Secret issued by Magnifi. Sent on every request alongside x-access-key.
  in: header
  name: AccessSecret
  parameter: x-access-secret
  sources:
  - openapi/videoverse-magnifi-partner-openapi.yml
  type: apiKey
slug: videoverse-authentication
source_filename: videoverse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/videoverse-magnifi-partner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessKey\n  type: apiKey\n  in: header\n  parameter: x-access-key\n  description: 'Partner Access Key issued by Magnifi. Documented example prefix: pak_.'\n  sources:\n  - openapi/videoverse-magnifi-partner-openapi.yml\n- name: AccessSecret\n  type: apiKey\n  in: header\n  parameter: x-access-secret\n  description: Partner Access Secret issued by Magnifi. Sent on every request alongside x-access-key.\n  sources:\n  - openapi/videoverse-magnifi-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/authentication/videoverse-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Video
- Artificial Intelligence
- Sports
- Media
- Broadcasting
- Video Editing
- Highlights
- Content Creation
- Machine-Learning
- Webhook
---
