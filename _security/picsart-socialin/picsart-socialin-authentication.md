---
api_key_in:
- header
api_specs:
- filename: picsart-socialin-image-tools.yaml
  format: yaml
  label: Picsart Programmable Image APIs
  slug: picsart-programmable-image-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart-socialin/refs/heads/main/openapi/picsart-socialin-image-tools.yaml
- filename: picsart-socialin-video-tools.yaml
  format: yaml
  label: Picsart Programmable Video APIs
  slug: picsart-programmable-video-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart-socialin/refs/heads/main/openapi/picsart-socialin-video-tools.yaml
- filename: picsart-socialin-genai-tools.yaml
  format: yaml
  label: Picsart GenAI API
  slug: picsart-genai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart-socialin/refs/heads/main/openapi/picsart-socialin-genai-tools.yaml
- filename: picsart-socialin-variable-data-tools.yaml
  format: yaml
  label: Picsart Variable Data Content APIs
  slug: picsart-variable-data-content-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart-socialin/refs/heads/main/openapi/picsart-socialin-variable-data-tools.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Picsart Socialin Authentication
name_suffix: Authentication
oauth_flows: []
overview: PicsArt (Socialin) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PicsArt (Socialin)
provider_slug: picsart-socialin
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Picsart-API-Key
  sources:
  - openapi/picsart-socialin-genai-tools.yaml
  - openapi/picsart-socialin-image-tools.yaml
  - openapi/picsart-socialin-variable-data-tools.yaml
  - openapi/picsart-socialin-video-tools.yaml
  type: apiKey
slug: picsart-socialin-authentication
source_filename: picsart-socialin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/picsart-socialin-genai-tools.yaml, openapi/picsart-socialin-image-tools.yaml,\n  openapi/picsart-socialin-variable-data-tools.yaml, openapi/picsart-socialin-video-tools.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Picsart-API-Key\n  sources:\n  - openapi/picsart-socialin-genai-tools.yaml\n  - openapi/picsart-socialin-image-tools.yaml\n  - openapi/picsart-socialin-variable-data-tools.yaml\n  - openapi/picsart-socialin-video-tools.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picsart-socialin/refs/heads/main/authentication/picsart-socialin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Image Editing
- Video Editing
- Generative AI
- Photo
- Creative Tools
- Image Processing
- Background Removal
- Machine Learning
- Content Generation
---
