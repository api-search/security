---
api_key_in: []
api_specs:
- filename: tray-ai-embedded-api-openapi.yml
  format: yaml
  label: Tray.ai Embedded API
  slug: embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-embedded-api-openapi.yml
- filename: tray-ai-platform-api-openapi.yml
  format: yaml
  label: Tray.ai Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tray Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tray.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tray.ai
provider_slug: tray-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Use either a master token (obtained from Tray Embedded UI settings) or a user token (obtained via the authorize mutation). Master tokens are required for admin operations like managing users. User tokens are required for user-scoped operations like managing solution instances.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tray-ai-embedded-api-openapi.yml
  - openapi/tray-ai-platform-api-openapi.yml
  type: http
slug: tray-ai-authentication
source_filename: tray-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tray-ai-embedded-api-openapi.yml, openapi/tray-ai-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Use either a master token (obtained from Tray Embedded UI settings) or a user\n    token (obtained via the authorize mutation). Master tokens are required for admin operations\n    like managing users. User tokens are required for user-scoped operations like managing solution\n    instances.\n  sources:\n  - openapi/tray-ai-embedded-api-openapi.yml\n  - openapi/tray-ai-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/authentication/tray-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Integration
- iPaaS
- AI Agents
- MCP
---
