---
api_key_in: []
api_specs:
- filename: obsidian-active-file-api-openapi.yml
  format: yaml
  label: Obsidian Active File API
  slug: obsidian-active-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-active-file-api-openapi.yml
- filename: obsidian-commands-api-openapi.yml
  format: yaml
  label: Obsidian Commands API
  slug: obsidian-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-commands-api-openapi.yml
- filename: obsidian-open-api-openapi.yml
  format: yaml
  label: Obsidian Open API
  slug: obsidian-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-open-api-openapi.yml
- filename: obsidian-periodic-notes-api-openapi.yml
  format: yaml
  label: Obsidian Periodic Notes API
  slug: obsidian-periodic-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-periodic-notes-api-openapi.yml
- filename: obsidian-search-api-openapi.yml
  format: yaml
  label: Obsidian Search API
  slug: obsidian-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-search-api-openapi.yml
- filename: obsidian-system-api-openapi.yml
  format: yaml
  label: Obsidian System API
  slug: obsidian-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-system-api-openapi.yml
- filename: obsidian-tags-api-openapi.yml
  format: yaml
  label: Obsidian Tags API
  slug: obsidian-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-tags-api-openapi.yml
- filename: obsidian-vault-directories-api-openapi.yml
  format: yaml
  label: Obsidian Vault Directories API
  slug: obsidian-vault-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-vault-directories-api-openapi.yml
- filename: obsidian-vault-files-api-openapi.yml
  format: yaml
  label: Obsidian Vault Files API
  slug: obsidian-vault-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-vault-files-api-openapi.yml
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
- Knowledge-Management
- Markdown
- Notes
- Local-First
---
