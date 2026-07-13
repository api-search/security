---
api_key_in: []
api_specs:
- filename: obsidian-local-rest-api-openapi.yaml
  format: yaml
  label: Obsidian Local REST API
  slug: obsidian-local-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-local-rest-api-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Obsidian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obsidian secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Obsidian
provider_slug: obsidian
scheme_count: 1
schemes:
- description: 'Find your API Key in your Obsidian settings

    in the "Local REST API" section under "Plugins".'
  name: apiKeyAuth
  scheme: bearer
  sources:
  - openapi/obsidian-local-rest-api-openapi.yaml
  type: http
slug: obsidian-authentication
source_filename: obsidian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/obsidian-local-rest-api-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Find your API Key in your Obsidian settings\n    in the \"Local REST API\" section under \"Plugins\".\n  sources:\n  - openapi/obsidian-local-rest-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/authentication/obsidian-authentication.yml
summary_line: http · 1 scheme
tags:
- Productivity
- Knowledge Management
- Markdown
- Notes
- Local-First
---
