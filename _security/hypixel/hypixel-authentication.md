---
api_key_in:
- header
api_specs:
- filename: hypixel-public-api-openapi.yml
  format: yaml
  label: Hypixel Public API
  slug: hypixel-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypixel/refs/heads/main/openapi/hypixel-public-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hypixel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hypixel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hypixel
provider_slug: hypixel
scheme_count: 1
schemes:
- description: Obtained via the [Hypixel Developer Dashboard](https://developer.hypixel.net) when creating an application. You can also request higher limits for production applications in this dashboard.
  in: header
  name: ApiKey
  parameter: API-Key
  sources:
  - openapi/hypixel-public-api-openapi.json
  - openapi/hypixel-public-api-openapi.yml
  type: apiKey
slug: hypixel-authentication
source_filename: hypixel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hypixel-public-api-openapi.json, openapi/hypixel-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: Obtained via the [Hypixel Developer Dashboard](https://developer.hypixel.net)\n    when creating an application. You can also request higher limits for production applications\n    in this dashboard.\n  sources:\n  - openapi/hypixel-public-api-openapi.json\n  - openapi/hypixel-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypixel/refs/heads/main/authentication/hypixel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Games And Comics
- Gaming
- Minecraft
- Player Stats
- Leaderboards
- SkyBlock
- Public APIs
---
