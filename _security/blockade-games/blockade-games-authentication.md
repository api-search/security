---
api_key_in:
- header
api_specs:
- filename: blockade-games-skybox-openapi.yml
  format: yaml
  label: Skybox AI API
  slug: skybox-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockade-games/refs/heads/main/openapi/blockade-games-skybox-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blockade Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockade Games secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blockade Games
provider_slug: blockade-games
scheme_count: 1
schemes:
- in: header
  name: default
  parameter: x-api-key
  sources:
  - openapi/blockade-games-skybox-openapi.yml
  type: apiKey
slug: blockade-games-authentication
source_filename: blockade-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/blockade-games-skybox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: default\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/blockade-games-skybox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockade-games/refs/heads/main/authentication/blockade-games-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Image Generation
- 3D
- Gaming
- Virtual Reality
- Content Generation
- Skybox
---
