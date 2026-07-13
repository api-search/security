---
api_key_in: []
api_specs:
- filename: gitpod-environments-openapi.yml
  format: yaml
  label: Gitpod Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitpod/refs/heads/main/openapi/gitpod-environments-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitpod Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gitpod secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gitpod
provider_slug: gitpod
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gitpod-environments-openapi.yml
  type: http
slug: gitpod-authentication
source_filename: gitpod-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitpod-environments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/gitpod-environments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitpod/refs/heads/main/authentication/gitpod-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Cloud Development Environments
- Workspaces
- AI Agents
- DevOps
---
