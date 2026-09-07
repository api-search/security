---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: videoverse-magnifi-partner-openapi.yml
  format: yaml
  label: Magnifi Partner Integration API
  slug: magnifi-partner-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoverse/refs/heads/main/openapi/videoverse-magnifi-partner-openapi.yml
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
- Machine Learning
- Webhooks
---
