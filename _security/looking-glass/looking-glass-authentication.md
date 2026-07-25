---
api_key_in: []
api_specs:
- filename: looking-glass-autostart-api-openapi.yml
  format: yaml
  label: Looking Glass Autostart API
  slug: looking-glass-autostart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-autostart-api-openapi.yml
- filename: looking-glass-devices-api-openapi.yml
  format: yaml
  label: Looking Glass Devices API
  slug: looking-glass-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-devices-api-openapi.yml
- filename: looking-glass-orchestration-api-openapi.yml
  format: yaml
  label: Looking Glass Orchestration API
  slug: looking-glass-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-orchestration-api-openapi.yml
- filename: looking-glass-playback-api-openapi.yml
  format: yaml
  label: Looking Glass Playback API
  slug: looking-glass-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-playback-api-openapi.yml
- filename: looking-glass-playlist-api-openapi.yml
  format: yaml
  label: Looking Glass Playlist API
  slug: looking-glass-playlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-playlist-api-openapi.yml
- filename: looking-glass-version-api-openapi.yml
  format: yaml
  label: Looking Glass Version API
  slug: looking-glass-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-version-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Looking Glass Authentication
name_suffix: Authentication
oauth_flows: []
overview: Looking Glass declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Looking Glass
provider_slug: looking-glass
scheme_count: 0
schemes: []
slug: looking-glass-authentication
source_filename: looking-glass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/Looking-Glass/bridge.js + openapi/looking-glass-bridge-openapi.yml\nsummary:\n  types: []\n  model: none\n  notes: >-\n    The Looking Glass Bridge HTTP REST API is a local loopback service\n    (http://localhost:33334/) with no authentication tokens or API keys. Access\n    control is by the trusted-origin loopback boundary — only processes on the\n    host machine can reach Bridge. Sessions are namespaced by an \"orchestration\"\n    token returned from enter_orchestration, but that token is a session\n    identifier for multi-app coordination, not an authentication credential.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/authentication/looking-glass-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Holographic Displays
- Light Field
- 3D
- Developer Tools
- WebXR
- Hardware
- Holograms
- Media Player
---
