---
api_key_in: []
api_specs:
- filename: tray-ai-authentication-api-openapi.yml
  format: yaml
  label: Tray.ai Authentication API
  slug: tray-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentication-api-openapi.yml
- filename: tray-ai-authentications-api-openapi.yml
  format: yaml
  label: Tray.ai Authentications API
  slug: tray-ai-authentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentications-api-openapi.yml
- filename: tray-ai-call-connector-api-openapi.yml
  format: yaml
  label: Tray.ai Call Connector API
  slug: tray-ai-call-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-call-connector-api-openapi.yml
- filename: tray-ai-connectors-api-openapi.yml
  format: yaml
  label: Tray.ai Connectors API
  slug: tray-ai-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-connectors-api-openapi.yml
- filename: tray-ai-deployments-api-openapi.yml
  format: yaml
  label: Tray.ai Deployments API
  slug: tray-ai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-deployments-api-openapi.yml
- filename: tray-ai-projects-api-openapi.yml
  format: yaml
  label: Tray.ai Projects API
  slug: tray-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-projects-api-openapi.yml
- filename: tray-ai-solution-instances-api-openapi.yml
  format: yaml
  label: Tray.ai Solution Instances API
  slug: tray-ai-solution-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solution-instances-api-openapi.yml
- filename: tray-ai-solutions-api-openapi.yml
  format: yaml
  label: Tray.ai Solutions API
  slug: tray-ai-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solutions-api-openapi.yml
- filename: tray-ai-triggers-api-openapi.yml
  format: yaml
  label: Tray.ai Triggers API
  slug: tray-ai-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-triggers-api-openapi.yml
- filename: tray-ai-users-api-openapi.yml
  format: yaml
  label: Tray.ai Users API
  slug: tray-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-users-api-openapi.yml
- filename: tray-ai-workflows-api-openapi.yml
  format: yaml
  label: Tray.ai Workflows API
  slug: tray-ai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workflows-api-openapi.yml
- filename: tray-ai-workspaces-api-openapi.yml
  format: yaml
  label: Tray.ai Workspaces API
  slug: tray-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workspaces-api-openapi.yml
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
