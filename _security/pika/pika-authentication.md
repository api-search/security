---
api_key_in:
- header
api_specs:
- filename: pika-text-to-video-openapi.yml
  format: yaml
  label: Pika Video API
  slug: pika-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pika/refs/heads/main/openapi/pika-text-to-video-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pika Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pika secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pika
provider_slug: pika
scheme_count: 1
schemes:
- description: Fal Key
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/pika-image-to-video-openapi.yml
  - openapi/pika-text-to-video-openapi.yml
  type: apiKey
slug: pika-authentication
source_filename: pika-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pika-image-to-video-openapi.yml, openapi/pika-text-to-video-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Fal Key\n  sources:\n  - openapi/pika-image-to-video-openapi.yml\n  - openapi/pika-text-to-video-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pika/refs/heads/main/authentication/pika-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Video Generation
- Text-to-Video
- Image-to-Video
- Diffusion Models
- Generative AI
- Media
- Creative Tools
---
