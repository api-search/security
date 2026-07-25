---
api_key_in: []
api_specs:
- filename: playcanvas-apps-api-openapi.yml
  format: yaml
  label: PlayCanvas Apps API
  slug: playcanvas-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-apps-api-openapi.yml
- filename: playcanvas-assets-api-openapi.yml
  format: yaml
  label: PlayCanvas Assets API
  slug: playcanvas-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-assets-api-openapi.yml
- filename: playcanvas-branches-api-openapi.yml
  format: yaml
  label: PlayCanvas Branches API
  slug: playcanvas-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-branches-api-openapi.yml
- filename: playcanvas-checkpoints-api-openapi.yml
  format: yaml
  label: PlayCanvas Checkpoints API
  slug: playcanvas-checkpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-checkpoints-api-openapi.yml
- filename: playcanvas-jobs-api-openapi.yml
  format: yaml
  label: PlayCanvas Jobs API
  slug: playcanvas-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-jobs-api-openapi.yml
- filename: playcanvas-projects-api-openapi.yml
  format: yaml
  label: PlayCanvas Projects API
  slug: playcanvas-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-projects-api-openapi.yml
- filename: playcanvas-ratelimits-api-openapi.yml
  format: yaml
  label: PlayCanvas RateLimits API
  slug: playcanvas-ratelimits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-ratelimits-api-openapi.yml
- filename: playcanvas-scenes-api-openapi.yml
  format: yaml
  label: PlayCanvas Scenes API
  slug: playcanvas-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-scenes-api-openapi.yml
- filename: playcanvas-splats-api-openapi.yml
  format: yaml
  label: PlayCanvas Splats API
  slug: playcanvas-splats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-splats-api-openapi.yml
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
