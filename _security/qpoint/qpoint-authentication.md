---
api_key_in:
- header
- cli-flag
auth_types:
- http-bearer
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Qpoint Authentication
name_suffix: Authentication
oauth_flows:
- firebase-auth
overview: Qpoint secures its APIs with http-bearer, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the firebase-auth flow(s).
provider_name: Qpoint
provider_slug: qpoint
scheme_count: 3
schemes:
- applies_to: MCP server (pulse.qpoint.io/mcp/v1)
  docs: https://docs.qpoint.io/guides/qplane-guides/mcp-getting-started.md
  in: header
  name: mcp-bearer
  note: Token minted in Qplane dashboard under Settings -> Deployments.
  parameter: Authorization
  scheme: bearer
  type: http
- applies_to: qtap agent registration with Qplane
  docs: https://docs.qpoint.io/getting-started/qtap/cli.md
  in: cli-flag
  name: registration-token
  parameter: --registration-token
  type: apiKey
- applies_to: Qplane web app (app.qpoint.io)
  name: qplane-app-auth
  note: Firebase Authentication; supports SSO for dashboard access per Security & Compliance docs.
  scheme: firebase-auth
  type: oauth2
slug: qpoint-authentication
source_filename: qpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qpoint.io/guides/qplane-guides/mcp-getting-started.md\n# No OpenAPI is published (Qpoint's control plane is gRPC/Connect + MCP), so this profile\n# is captured from the docs rather than derived from a spec.\nsummary:\n  types: [http-bearer, apiKey, oauth2]\n  api_key_in: [header, cli-flag]\n  oauth2_flows: [firebase-auth]\nschemes:\n- name: mcp-bearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  applies_to: MCP server (pulse.qpoint.io/mcp/v1)\n  docs: https://docs.qpoint.io/guides/qplane-guides/mcp-getting-started.md\n  note: Token minted in Qplane dashboard under Settings -> Deployments.\n- name: registration-token\n  type: apiKey\n  in: cli-flag\n  parameter: --registration-token\n  applies_to: qtap agent registration with Qplane\n  docs: https://docs.qpoint.io/getting-started/qtap/cli.md\n- name: qplane-app-auth\n  type: oauth2\n  scheme: firebase-auth\n  applies_to: Qplane web\
  \ app (app.qpoint.io)\n  note: Firebase Authentication; supports SSO for dashboard access per Security & Compliance docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qpoint/refs/heads/main/authentication/qpoint-authentication.yml
summary_line: http-bearer/apiKey/oauth2 · 3 schemes
tags:
- Company
- Security
- Observability
- eBPF
- Network Traffic
- Egress Control
- Agentic AI
- MCP
- gRPC
---
