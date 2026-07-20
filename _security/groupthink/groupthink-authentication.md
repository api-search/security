---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Groupthink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groupthink secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Groupthink
provider_slug: groupthink
scheme_count: 1
schemes:
- description: Groupthink API tokens are Bearer credentials minted in the app under Settings -> API Tokens. A token is displayed only once at creation and can be revoked immediately, which blocks all client access. Sent on the Authorization request header as "Bearer <token>".
  header_name: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  sources:
  - docs/mcp_server
  token_management_url: https://app.groupthink.com/
  type: http
slug: groupthink-authentication
source_filename: groupthink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://groupthink.com/docs/mcp_server/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    description: >-\n      Groupthink API tokens are Bearer credentials minted in the app under\n      Settings -> API Tokens. A token is displayed only once at creation and can\n      be revoked immediately, which blocks all client access. Sent on the\n      Authorization request header as \"Bearer <token>\".\n    in: header\n    header_name: Authorization\n    token_management_url: https://app.groupthink.com/\n    sources: [docs/mcp_server]\nnotes: >-\n  Derived from the published MCP server documentation (no OpenAPI securitySchemes\n  are published). Groupthink also supports a bring-your-own Anthropic API key for\n  meeting summaries, which is a per-user LLM credential, not an API auth scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupthink/refs/heads/main/authentication/groupthink-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SaaS
- Meetings
- Transcription
- Note Taking
- Relationship Intelligence
- MCP
- AI Assistant
- Productivity
- CRM
---
