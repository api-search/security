---
api_key_in: []
api_specs:
- filename: graphy-agents-openapi.yaml
  format: yaml
  label: Graphy AI Agents API
  slug: graphy-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphy/refs/heads/main/openapi/graphy-agents-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Graphy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graphy
provider_slug: graphy
scheme_count: 1
schemes:
- description: Your Graphy API key (starts with graphy_). Create one in the Graphy console at https://agents.graphy.dev/console/. Keys must be kept out of frontend code and stored via environment variables or a secrets manager. All requests also require Content-Type application/json.
  format: Bearer [example key]
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/graphy-agents-openapi.yaml
  type: http
slug: graphy-authentication
source_filename: graphy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/graphy-agents-openapi.yaml\ndocs: https://docs.graphy.dev/agents/rest/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_prefix: graphy_\n  key_console: https://agents.graphy.dev/console/\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer [example key]'\n  description: Your Graphy API key (starts with graphy_). Create one in the Graphy console at\n    https://agents.graphy.dev/console/. Keys must be kept out of frontend code and stored via\n    environment variables or a secrets manager. All requests also require Content-Type application/json.\n  sources:\n  - openapi/graphy-agents-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphy/refs/heads/main/authentication/graphy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Visualization
- Charts
- Charting
- Analytics
- Artificial Intelligence
- Data Storytelling
- Developer Tools
- SDK
- Agents
---
