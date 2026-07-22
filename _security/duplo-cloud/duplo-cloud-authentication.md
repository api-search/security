---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Duplo Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duplo Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duplo Cloud
provider_slug: duplo-cloud
scheme_count: 1
schemes:
- description: DuploCloud REST API and MCP server requests authenticate with a User Token (a personal access token) minted per user under Access Control > User Tokens, presented as an HTTP Bearer token. The same token authorizes duploctl (the Python SDK/CLI), the Terraform provider, and the MCP server.
  format: 'Authorization: Bearer <token>'
  header: Authorization
  in: header
  name: userToken
  scheme: bearer
  sources:
  - docs
  type: http
slug: duplo-cloud-authentication
source_filename: duplo-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.duplocloud.com/docs/armor/access-control/user-tokens.md\ndocs: https://docs.duplocloud.com/docs/armor/access-control/user-tokens.md\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: userToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <token>'\n    description: >-\n      DuploCloud REST API and MCP server requests authenticate with a User Token\n      (a personal access token) minted per user under Access Control > User Tokens,\n      presented as an HTTP Bearer token. The same token authorizes duploctl (the\n      Python SDK/CLI), the Terraform provider, and the MCP server.\n    sources: [docs]\nnotes: >-\n  DuploCloud is deployed as a dedicated per-customer portal, so the API base URL is\n  organization-specific (e.g. https://<portal>.duplocloud.net). Authorization,\n  permission\
  \ sets, user groups, and AI guardrails are managed in the platform's\n  Access Control surface rather than via OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duplo-cloud/refs/heads/main/authentication/duplo-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- DevOps
- Cloud Infrastructure
- Infrastructure as Code
- Security and Compliance
- AI Agents
- Kubernetes
- Automation
---
