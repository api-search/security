---
api_key_in: []
api_specs:
- filename: colossyan-avatars-api-openapi.yml
  format: yaml
  label: Colossyan Avatars API
  slug: colossyan-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-avatars-api-openapi.yml
- filename: colossyan-experimental-api-openapi.yml
  format: yaml
  label: Colossyan Experimental API
  slug: colossyan-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-experimental-api-openapi.yml
- filename: colossyan-generated-videos-api-openapi.yml
  format: yaml
  label: Colossyan Generated Videos API
  slug: colossyan-generated-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-generated-videos-api-openapi.yml
- filename: colossyan-video-generation-api-openapi.yml
  format: yaml
  label: Colossyan Video Generation API
  slug: colossyan-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-video-generation-api-openapi.yml
- filename: colossyan-voices-api-openapi.yml
  format: yaml
  label: Colossyan Voices API
  slug: colossyan-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-voices-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Colossyan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Colossyan secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Colossyan
provider_slug: colossyan
scheme_count: 1
schemes:
- description: Bearer token authentication. Provide the workspace API token in the Authorization header as `Bearer {token}`. The token is available in the workspace Settings and requires a Business or Enterprise plan.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/colossyan-openapi.yml
  type: http
slug: colossyan-authentication
source_filename: colossyan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/colossyan-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Provide the workspace API token in the Authorization\n    header as `Bearer {token}`. The token is available in the workspace Settings and requires\n    a Business or Enterprise plan.\n  sources:\n  - openapi/colossyan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/authentication/colossyan-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Video Generation
- Avatars
- Text to Video
- Learning and Development
---
