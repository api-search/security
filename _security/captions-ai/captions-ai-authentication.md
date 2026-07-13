---
api_key_in:
- header
api_specs:
- filename: add-captions-to-a-video
  format: yaml
  label: Captions Video Captions API
  slug: captions-ai-video-captions-api
  spec_type: OpenAPI
  url: https://captions.ai/help/api-reference/video-captions/add-captions-to-a-video
- filename: captions-ai-creator-ads-openapi.yml
  format: yaml
  label: Captions AI Creator API
  slug: captions-ai-creator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-creator-ads-openapi.yml
- filename: captions-ai-creator-ads-openapi.yml
  format: yaml
  label: Captions AI Ads API
  slug: captions-ai-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-creator-ads-openapi.yml
- filename: captions-ai-mirage-video-openapi.yml
  format: yaml
  label: Mirage Video Generation API
  slug: captions-mirage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-mirage-video-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Captions Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Captions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Captions
provider_slug: captions-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/captions-ai-creator-ads-openapi.yml
  - openapi/captions-ai-mirage-video-openapi.yml
  type: apiKey
slug: captions-ai-authentication
source_filename: captions-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/captions-ai-creator-ads-openapi.yml, openapi/captions-ai-mirage-video-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/captions-ai-creator-ads-openapi.yml\n  - openapi/captions-ai-mirage-video-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/authentication/captions-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Video
- Video Generation
- Video Captioning
- AI Dubbing
- Lip Sync
- AI Twin
- Text to Video
- Generative AI
- Video Translation
---
