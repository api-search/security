---
api_key_in:
- url
auth_types:
- connection-url
description: ''
kind: authentication
layout: security
method: searched
name: Syncly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syncly secures its APIs with connection-url across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Syncly
provider_slug: syncly
scheme_count: 1
schemes:
- description: Programmatic access to a Syncly workspace is authenticated with a per-workspace MCP connection URL copied from workspace settings (General > MCP URL panel). The URL carries a workspace-scoped token; it must be kept secret and is not shared externally. There is no public REST/OpenAPI API, API key issuance flow, or OAuth surface documented.
  in: url
  name: WorkspaceMcpConnectionUrl
  sources:
  - https://syncly-a76215af.mintlify.app/en/start/connect-mcp-clients
  type: connection-url
slug: syncly-authentication
source_filename: syncly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://syncly-a76215af.mintlify.app/en/start/connect-mcp-clients\ndocs: https://syncly-a76215af.mintlify.app/en/start/connect-mcp-clients\nsummary:\n  types: [connection-url]\n  api_key_in: [url]\n  oauth2_flows: []\nschemes:\n  - name: WorkspaceMcpConnectionUrl\n    type: connection-url\n    in: url\n    description: >-\n      Programmatic access to a Syncly workspace is authenticated with a\n      per-workspace MCP connection URL copied from workspace settings\n      (General > MCP URL panel). The URL carries a workspace-scoped token;\n      it must be kept secret and is not shared externally. There is no public\n      REST/OpenAPI API, API key issuance flow, or OAuth surface documented.\n    sources: [https://syncly-a76215af.mintlify.app/en/start/connect-mcp-clients]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/authentication/syncly-authentication.yml
summary_line: connection-url · 1 scheme
tags:
- Company
- Social Intelligence
- Social Listening
- Customer Feedback
- Voice of Customer
- Creator Marketing
- Analytics
- Artificial Intelligence
- MCP
---
