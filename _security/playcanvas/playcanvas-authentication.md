---
api_key_in: []
api_specs:
- filename: playcanvas-rest-openapi.yml
  format: yaml
  label: PlayCanvas REST API
  slug: playcanvas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-rest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Playcanvas Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlayCanvas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PlayCanvas
provider_slug: playcanvas
scheme_count: 1
schemes:
- description: 'Access token generated on the Organization Account page, sent as `Authorization: Bearer {accessToken}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/playcanvas-rest-openapi.yml
  type: http
slug: playcanvas-authentication
source_filename: playcanvas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/playcanvas-rest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token generated on the Organization Account page, sent as `Authorization:\n    Bearer {accessToken}`.'\n  sources:\n  - openapi/playcanvas-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/authentication/playcanvas-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- 3D
- Game Engine
- WebGL
- WebGPU
- Graphics
- Developer Tools
- Gaussian Splatting
- Rendering
---
