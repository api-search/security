---
api_key_in: []
api_specs:
- filename: runwayml-character-performance-api-openapi.yml
  format: yaml
  label: Runway Character Performance API
  slug: runwayml-character-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-character-performance-api-openapi.yml
- filename: runwayml-image-to-video-api-openapi.yml
  format: yaml
  label: Runway Image-to-Video API
  slug: runwayml-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-image-to-video-api-openapi.yml
- filename: runwayml-organization-api-openapi.yml
  format: yaml
  label: Runway Organization API
  slug: runwayml-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-organization-api-openapi.yml
- filename: runwayml-tasks-api-openapi.yml
  format: yaml
  label: Runway Tasks API
  slug: runwayml-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-tasks-api-openapi.yml
- filename: runwayml-text-to-image-api-openapi.yml
  format: yaml
  label: Runway Text-to-Image API
  slug: runwayml-text-to-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-text-to-image-api-openapi.yml
- filename: runwayml-text-to-speech-api-openapi.yml
  format: yaml
  label: Runway Text-to-Speech API
  slug: runwayml-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-text-to-speech-api-openapi.yml
- filename: runwayml-upscale-api-openapi.yml
  format: yaml
  label: Runway Upscale API
  slug: runwayml-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-upscale-api-openapi.yml
- filename: runwayml-video-to-video-api-openapi.yml
  format: yaml
  label: Runway Video-to-Video API
  slug: runwayml-video-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-video-to-video-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runwayml Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runway
provider_slug: runwayml
scheme_count: 1
schemes:
- description: Runway API key issued via the Runway Developer Portal, supplied as a bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runway-ml-openapi.yml
  type: http
slug: runwayml-authentication
source_filename: runwayml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runway-ml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Runway API key issued via the Runway Developer Portal, supplied as a bearer token\n    in the Authorization header.\n  sources:\n  - openapi/runway-ml-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/authentication/runwayml-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- Text-to-Image
- Video-to-Video
---
