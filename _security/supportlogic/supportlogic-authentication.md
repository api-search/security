---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Supportlogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supportlogic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Supportlogic
provider_slug: supportlogic
scheme_count: 1
schemes:
- description: Tenant-scoped bearer token generated in the SupportLogic Command Center (Settings -> MCP Server -> Generate Credentials) and presented to the hosted MCP endpoint. This is the only publicly documented authentication mechanism; SupportLogic publishes no public OpenAPI or OAuth2 authorization server.
  docs: https://www.supportlogic.com/platform/mcp-server/
  name: bearerToken
  scheme: bearer
  sources:
  - mcp/supportlogic-mcp.yml
  type: http
slug: supportlogic-authentication
source_filename: supportlogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.supportlogic.com/platform/mcp-server/\nsummary:\n  types: [http]\n  api_key_in: []\n  http_schemes: [bearer]\n  oauth2_flows: []\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Tenant-scoped bearer token generated in the SupportLogic Command Center\n    (Settings -> MCP Server -> Generate Credentials) and presented to the hosted\n    MCP endpoint. This is the only publicly documented authentication mechanism;\n    SupportLogic publishes no public OpenAPI or OAuth2 authorization server.\n  sources: [mcp/supportlogic-mcp.yml]\n  docs: https://www.supportlogic.com/platform/mcp-server/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supportlogic/refs/heads/main/authentication/supportlogic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Support
- Customer Experience
- Artificial Intelligence
- Service Experience
- Sentiment Analysis
- Escalation Management
- MCP
- SaaS
---
