---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Software secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Software
provider_slug: software
scheme_count: 1
schemes:
- description: Enterprise Access Token minted in the Antenna app (enterprise settings → Access Tokens → Create token), shown once. Authorizes read-only calls to the hosted MCP server at https://app.antenna.dev/api/mcp/enterprise. Scoped to the caller's enterprise; requires the MCP feature enabled.
  format: Bearer <token>
  header: Authorization
  in: header
  name: EnterpriseAccessToken
  scheme: bearer
  sources:
  - https://docs.antenna.dev/mcp-server
  type: http
slug: software-authentication
source_filename: software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.antenna.dev/mcp-server\ndocs: https://docs.antenna.dev/mcp-server\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Antenna has no published OpenAPI. Auth model captured from the MCP-server\n    and quickstart documentation. Programmatic access (the hosted MCP / metrics\n    API) uses a Bearer \"Enterprise Access Token\"; the web console uses SSO.\nschemes:\n- name: EnterpriseAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n  description: >-\n    Enterprise Access Token minted in the Antenna app (enterprise settings →\n    Access Tokens → Create token), shown once. Authorizes read-only calls to\n    the hosted MCP server at https://app.antenna.dev/api/mcp/enterprise. Scoped\n    to the caller's enterprise; requires the MCP feature enabled.\n  sources: [https://docs.antenna.dev/mcp-server]\n\
  console_sso:\n  description: >-\n    End-user sign-in to the Antenna web application uses enterprise Single\n    Sign-On.\n  providers:\n  - Okta Single Sign-On\n  - Microsoft Entra Single Sign-On\n  source: https://docs.antenna.dev/get-started/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software/refs/heads/main/authentication/software-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Productivity
- Engineering Intelligence
- AI
- Software Development
- Analytics
- Metrics
- DORA
- MCP
- Developer Experience
---
