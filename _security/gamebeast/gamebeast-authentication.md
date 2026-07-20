---
api_key_in:
- config
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gamebeast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gamebeast secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gamebeast
provider_slug: gamebeast
scheme_count: 2
schemes:
- audience: client-side / in-game SDK
  capabilities:
  - Send engagement markers
  - Read remote configurations
  - Read / assign experiments
  - Read user cohorts
  - Create / read heatmaps
  name: SDK Key (public)
  scope: project
  sources:
  - https://docs.gamebeast.gg/Features/ApiKeys
  type: apiKey
  usage:
    roblox: Gamebeast:Setup({ key = "..." })
    unity: GamebeastSdk.Init("...")
- audience: server-to-server / backend
  capabilities:
  - Analytics and query operations
  - GDPR deletion requests
  - Marker metadata queries
  - (superset of SDK Key capabilities)
  handling: Secret shown only once on creation/rotation; never embed in client code or public repositories; rotate immediately if exposed.
  name: Server Key (private)
  scope: organization
  sources:
  - https://docs.gamebeast.gg/Features/ApiKeys
  type: apiKey
slug: gamebeast-authentication
source_filename: gamebeast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gamebeast.gg/Features/ApiKeys\ndocs: https://docs.gamebeast.gg/Features/ApiKeys\nsummary:\n  types: [apiKey]\n  api_key_in: [config, header]\n  oauth2_flows: []\n  note: >-\n    Gamebeast uses API-key authentication (no OAuth). Keys are created, shown once,\n    and rotated in the dashboard (https://dashboard.gamebeast.gg). There are two\n    distinct key classes with different scope.\nschemes:\n  - name: SDK Key (public)\n    type: apiKey\n    scope: project\n    audience: client-side / in-game SDK\n    capabilities:\n      - Send engagement markers\n      - Read remote configurations\n      - Read / assign experiments\n      - Read user cohorts\n      - Create / read heatmaps\n    usage:\n      roblox: 'Gamebeast:Setup({ key = \"...\" })'\n      unity: 'GamebeastSdk.Init(\"...\")'\n    sources: [https://docs.gamebeast.gg/Features/ApiKeys]\n  - name: Server Key (private)\n    type: apiKey\n    scope: organization\n\
  \    audience: server-to-server / backend\n    capabilities:\n      - Analytics and query operations\n      - GDPR deletion requests\n      - Marker metadata queries\n      - (superset of SDK Key capabilities)\n    handling: >-\n      Secret shown only once on creation/rotation; never embed in client code or\n      public repositories; rotate immediately if exposed.\n    sources: [https://docs.gamebeast.gg/Features/ApiKeys]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamebeast/refs/heads/main/authentication/gamebeast-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Analytics
- Gaming
- Game Development
- LiveOps
- Experiments
- A/B Testing
- Roblox
- Unity
- Player Analytics
- Attribution
---
