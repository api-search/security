---
api_key_in:
- header
api_specs:
- filename: curse-categories-api-openapi.yml
  format: yaml
  label: Curse Categories API
  slug: curse-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-categories-api-openapi.yml
- filename: curse-files-api-openapi.yml
  format: yaml
  label: Curse Files API
  slug: curse-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-files-api-openapi.yml
- filename: curse-fingerprints-api-openapi.yml
  format: yaml
  label: Curse Fingerprints API
  slug: curse-fingerprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-fingerprints-api-openapi.yml
- filename: curse-games-api-openapi.yml
  format: yaml
  label: Curse Games API
  slug: curse-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-games-api-openapi.yml
- filename: curse-minecraft-api-openapi.yml
  format: yaml
  label: Curse Minecraft API
  slug: curse-minecraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-minecraft-api-openapi.yml
- filename: curse-mods-api-openapi.yml
  format: yaml
  label: Curse Mods API
  slug: curse-mods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-mods-api-openapi.yml
- filename: curse-subscriptions-api-openapi.yml
  format: yaml
  label: Curse Subscriptions API
  slug: curse-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-subscriptions-api-openapi.yml
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
- MODS
- Minecraft
- Game Content
- Developer Platform
- Catalog
---
