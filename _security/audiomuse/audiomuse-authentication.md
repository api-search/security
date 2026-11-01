---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Audiomuse Authentication
name_suffix: Authentication
oauth_flows: []
overview: AudioMuse-AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AudioMuse-AI
provider_slug: audiomuse
scheme_count: 2
schemes:
- description: 'API_TOKEN provided in Authorization: Bearer header for machine-to-machine callers.'
  scheme: bearer
  type: http
- description: Session authentication via JWT cookie set after login page.
  in: cookie
  name: JWT
  type: apiKey
slug: audiomuse-authentication
source_filename: audiomuse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://raw.githubusercontent.com/NeptuneHub/AudioMuse-AI/main/docs/AUTH.md\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"API_TOKEN provided in Authorization: Bearer header for machine-to-machine callers.\"\n  - type: apiKey\n    in: cookie\n    name: JWT\n    description: \"Session authentication via JWT cookie set after login page.\"\n"
source_yaml_url: https://artifacts.apis.io/audiomuse/authentication/audiomuse-authentication.yml
summary_line: 2 schemes
tags:
- Music
- AI
- OpenSource
- Self-Hosted
- Playlist
- AudioAnalysis
---
