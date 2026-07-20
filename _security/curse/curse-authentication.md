---
api_key_in:
- header
api_specs:
- filename: curse-core-openapi-original.yml
  format: yaml
  label: CurseForge Core API
  slug: curse-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-core-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Curse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Curse
provider_slug: curse
scheme_count: 1
schemes:
- description: <br/>The API key can be generated in the CurseForge for Studios [developer console](https://console.curseforge.com/).
  in: header
  name: API_KEY
  parameter: x-api-key
  sources:
  - openapi/curse-core-openapi-original.yml
  type: apiKey
slug: curse-authentication
source_filename: curse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/curse-core-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API_KEY\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: <br/>The API key can be generated in the CurseForge for Studios [developer console](https://console.curseforge.com/).\n  sources:\n  - openapi/curse-core-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/authentication/curse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Gaming
- Mods
- Minecraft
- Game Content
- Developer Platform
- Catalog
---
