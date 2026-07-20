---
api_key_in: []
api_specs:
- filename: continue-dev-hub-ide-api-openapi.yml
  format: yaml
  label: Continue Hub IDE API
  slug: continue-hub-ide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/openapi/continue-dev-hub-ide-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Continue Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Continue secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Continue
provider_slug: continue-dev
scheme_count: 1
schemes:
- description: 'API Key Authentication


    API keys must be prefixed with "con_" and provided in the Authorization header.

    Example: `Authorization: Bearer [example key]`


    API keys can be generated in the Continue Hub web interface under account settings.'
  name: apiKeyAuth
  scheme: bearer
  sources:
  - openapi/continue-dev-hub-ide-api-openapi.yml
  type: http
slug: continue-dev-authentication
source_filename: continue-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/continue-dev-hub-ide-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API Key Authentication\n\n    API keys must be prefixed with \"con_\" and provided in the Authorization header.\n    Example: `Authorization: Bearer [example key]`\n\n    API keys can be generated in the Continue Hub web interface under account settings.\n  sources:\n  - openapi/continue-dev-hub-ide-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/authentication/continue-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Developer Tools
- Code Assistant
- Open Source
- VS Code
- JetBrains
- CLI
- MCP
- Apache 2.0
---
