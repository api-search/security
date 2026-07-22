---
api_key_in: []
api_specs:
- filename: swagger-ui
  format: yaml
  label: System Initiative Public API
  slug: system-initiative-public-api
  spec_type: OpenAPI
  url: https://api.systeminit.com/swagger-ui
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: System Initiative Authentication
name_suffix: Authentication
oauth_flows: []
overview: System Initiative secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: System Initiative
provider_slug: system-initiative
scheme_count: 1
schemes:
- description: 'All System Initiative Public API endpoints require a workspace-scoped API token, passed as `Authorization: Bearer <token>`. Tokens are minted per workspace from the web application. Requests also target a specific workspace id (e.g. `SI_WORKSPACE_ID`), so a token + workspace id pair scopes every call.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.systeminit.com/how-tos/use-public-api
  type: http
slug: system-initiative-authentication
source_filename: system-initiative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.systeminit.com/how-tos/use-public-api\ndocs: https://docs.systeminit.com/reference/public-api\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_model: workspace-scoped API token (personal/automation token)\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      All System Initiative Public API endpoints require a workspace-scoped API\n      token, passed as `Authorization: Bearer <token>`. Tokens are minted per\n      workspace from the web application. Requests also target a specific\n      workspace id (e.g. `SI_WORKSPACE_ID`), so a token + workspace id pair\n      scopes every call.\n    sources: [https://docs.systeminit.com/how-tos/use-public-api]\nenv:\n  - SI_API_TOKEN\n  - SI_WORKSPACE_ID\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/system-initiative/refs/heads/main/authentication/system-initiative-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Infrastructure Automation
- DevOps
- Infrastructure as Code
- AI Agents
- Cloud
- MCP
---
