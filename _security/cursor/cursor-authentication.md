---
api_key_in: []
api_specs:
- filename: cursor-admin-api-openapi.yml
  format: yaml
  label: Cursor Admin API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-admin-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cursor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cursor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cursor
provider_slug: cursor
scheme_count: 1
schemes:
- description: Basic Authentication with API key as the username and empty password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cursor-admin-api-openapi.yml
  type: http
slug: cursor-authentication
source_filename: cursor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cursor-admin-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic Authentication with API key as the username and empty password.\n  sources:\n  - openapi/cursor-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/authentication/cursor-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Developer Tools
- Code Editor
- Agent
- IDE
- Cloud Agents
---
