---
api_key_in: []
api_specs:
- filename: runway-video-generation-openapi.yml
  format: yaml
  label: Runway Video Generation API
  slug: video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-video-generation-openapi.yml
- filename: runway-image-generation-openapi.yml
  format: yaml
  label: Runway Image Generation API
  slug: image-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-image-generation-openapi.yml
- filename: runway-characters-openapi.yml
  format: yaml
  label: Runway Characters API
  slug: characters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-characters-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runway
provider_slug: runway
scheme_count: 1
schemes:
- description: API key passed via the HTTP Authorization header using the Bearer scheme. Obtain your API key from the Runway Developer Portal at https://dev.runwayml.com/.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runway-characters-openapi.yml
  - openapi/runway-image-generation-openapi.yml
  - openapi/runway-video-generation-openapi.yml
  type: http
slug: runway-authentication
source_filename: runway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runway-characters-openapi.yml, openapi/runway-image-generation-openapi.yml,\n  openapi/runway-video-generation-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed via the HTTP Authorization header using the Bearer scheme. Obtain\n    your API key from the Runway Developer Portal at https://dev.runwayml.com/.\n  sources:\n  - openapi/runway-characters-openapi.yml\n  - openapi/runway-image-generation-openapi.yml\n  - openapi/runway-video-generation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/authentication/runway-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Generation
- Image Generation
- Artificial Intelligence
- Machine Learning
- Generative AI
- Avatars
- Characters
- WebRTC
- Creative Tools
---
