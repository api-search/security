---
api_key_in: []
api_specs:
- filename: looking-glass-bridge-openapi.yml
  format: yaml
  label: Looking Glass Bridge API
  slug: looking-glass-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-bridge-openapi.yml
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
