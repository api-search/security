---
api_key_in: []
api_specs:
- filename: spot-devices-openapi.json
  format: json
  label: Spot AI — Devices
  slug: spot-ai-devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-devices-openapi.json
- filename: spot-intelligence-openapi.json
  format: json
  label: Spot AI — Intelligence
  slug: spot-ai-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-intelligence-openapi.json
- filename: spot-connect-openapi.json
  format: json
  label: Spot AI — Spot Connect (beta)
  slug: spot-ai-spot-connect-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-connect-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Spot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spot
provider_slug: spot
scheme_count: 1
schemes:
- name: bearer_security
  scheme: bearer
  sources:
  - openapi/spot-connect-openapi.json
  - openapi/spot-devices-openapi.json
  - openapi/spot-intelligence-openapi.json
  type: http
slug: spot-authentication
source_filename: spot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spot-connect-openapi.json, openapi/spot-devices-openapi.json, openapi/spot-intelligence-openapi.json\ndocs: https://developers.spot.ai/reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nnotes: >-\n  Spot AI uses a bearer API key. An organization admin generates an API key on\n  the API settings page of the Spot dashboard (Create New Key -> name it ->\n  optional expiration, defaults to 1 year -> Generate Key). The key is shown\n  only once at creation. Keys are authorized by role (Owner recommended for full\n  access) with an optional resource scope. The key is sent as an HTTP bearer\n  token. Individual operations further require named permissions (e.g.\n  camera_share_create, clip_share_create, camera.manage_audio).\nschemes:\n- name: bearer_security\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/spot-connect-openapi.json\n  - openapi/spot-devices-openapi.json\n  - openapi/spot-intelligence-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/authentication/spot-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video
- Physical Security
- Surveillance
- Computer Vision
- Artificial Intelligence
- Cameras
- Analytics
- License Plate Recognition
- Webhooks
- Integrations
---
