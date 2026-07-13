---
api_key_in:
- header
api_specs:
- filename: ready-player-me-avatars-api-openapi.yml
  format: yaml
  label: Ready Player Me Avatars API
  slug: ready-player-me-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/openapi/ready-player-me-avatars-api-openapi.yml
- filename: ready-player-me-assets-api-openapi.yml
  format: yaml
  label: Ready Player Me Assets API
  slug: ready-player-me-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/openapi/ready-player-me-assets-api-openapi.yml
- filename: ready-player-me-auth-api-openapi.yml
  format: yaml
  label: Ready Player Me Auth API
  slug: ready-player-me-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/openapi/ready-player-me-auth-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ready Player Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ready Player Me secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ready Player Me
provider_slug: ready-player-me
scheme_count: 1
schemes:
- in: header
  name: AppId
  parameter: X-APP-ID
  sources:
  - openapi/ready-player-me-assets-api-openapi.yml
  - openapi/ready-player-me-avatars-api-openapi.yml
  type: apiKey
slug: ready-player-me-authentication
source_filename: ready-player-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ready-player-me-assets-api-openapi.yml, openapi/ready-player-me-avatars-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppId\n  type: apiKey\n  in: header\n  parameter: X-APP-ID\n  sources:\n  - openapi/ready-player-me-assets-api-openapi.yml\n  - openapi/ready-player-me-avatars-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/authentication/ready-player-me-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Avatars
- 3D
- Gaming
- VR
- AR
- Metaverse
- glTF
- Cross-Platform
- Unity
- Unreal
- Web
- Mobile
---
