---
api_key_in:
- header
api_specs:
- filename: picsart-image-tools-api-openapi-original.yml
  format: yaml
  label: Picsart Programmable Image APIs
  slug: picsart-programmable-image-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart/refs/heads/main/openapi/picsart-image-tools-api-openapi-original.yml
- filename: picsart-video-tools-api-openapi-original.yml
  format: yaml
  label: Picsart Programmable Video APIs
  slug: picsart-programmable-video-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart/refs/heads/main/openapi/picsart-video-tools-api-openapi-original.yml
- filename: picsart-genai-tools-api-openapi-original.yml
  format: yaml
  label: Picsart GenAI API
  slug: picsart-genai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart/refs/heads/main/openapi/picsart-genai-tools-api-openapi-original.yml
- filename: picsart-variable-data-tools-api-openapi-original.yml
  format: yaml
  label: Picsart Variable Data Content APIs
  slug: picsart-variable-data-content-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picsart/refs/heads/main/openapi/picsart-variable-data-tools-api-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Picsart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Picsart secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Picsart
provider_slug: picsart
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Picsart-API-Key
  sources:
  - openapi/picsart-genai-tools-api-openapi-original.yml
  - openapi/picsart-image-tools-api-openapi-original.yml
  - openapi/picsart-variable-data-tools-api-openapi-original.yml
  - openapi/picsart-video-tools-api-openapi-original.yml
  type: apiKey
slug: picsart-authentication
source_filename: picsart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/picsart-genai-tools-api-openapi-original.yml, openapi/picsart-image-tools-api-openapi-original.yml,\n  openapi/picsart-variable-data-tools-api-openapi-original.yml, openapi/picsart-video-tools-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Picsart-API-Key\n  sources:\n  - openapi/picsart-genai-tools-api-openapi-original.yml\n  - openapi/picsart-image-tools-api-openapi-original.yml\n  - openapi/picsart-variable-data-tools-api-openapi-original.yml\n  - openapi/picsart-video-tools-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picsart/refs/heads/main/authentication/picsart-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Images
- Image Processing
- Video
- Generative AI
- Machine Learning
- Media
- Content Creation
- Developer Tools
---
