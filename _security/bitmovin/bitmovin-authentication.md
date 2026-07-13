---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Bitmovin Encoding API
  slug: encoding-api
  spec_type: OpenAPI
  url: https://developer.bitmovin.com/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bitmovin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitmovin secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bitmovin
provider_slug: bitmovin
scheme_count: 2
schemes:
- description: Your Bitmovin API key
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/bitmovin-encoding-api-openapi.yml
  - openapi/bitmovin-platform-openapi.yml
  type: apiKey
- description: Your Bitmovin account organization
  in: header
  name: TenantOrgId
  parameter: X-Tenant-Org-Id
  sources:
  - openapi/bitmovin-encoding-api-openapi.yml
  - openapi/bitmovin-platform-openapi.yml
  type: apiKey
slug: bitmovin-authentication
source_filename: bitmovin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitmovin-encoding-api-openapi.yml, openapi/bitmovin-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Your Bitmovin API key\n  sources:\n  - openapi/bitmovin-encoding-api-openapi.yml\n  - openapi/bitmovin-platform-openapi.yml\n- name: TenantOrgId\n  type: apiKey\n  in: header\n  parameter: X-Tenant-Org-Id\n  description: Your Bitmovin account organization\n  sources:\n  - openapi/bitmovin-encoding-api-openapi.yml\n  - openapi/bitmovin-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/authentication/bitmovin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Video
- Encoding
- Streaming
- Live Streaming
- VOD
- Adaptive Bitrate
- HLS
- DASH
- DRM
- Player
- Analytics
- Media
- Cloud
---
