---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CreatorsCompanion Authentication
name_suffix: Authentication
oauth_flows: []
overview: CreatorsCompanion declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CreatorsCompanion
provider_slug: creatorscompanion-app
scheme_count: 1
schemes:
- applies_to: https://www.creatorscompanion.app/mcp
  authorization_servers:
  - https://loepapuzvunejbjoxixw.supabase.co/auth/v1
  bearer_methods_supported:
  - header
  description: Remote MCP over HTTP with OAuth. The first time you use it, your AI app opens a CreatorsCompanion page where you sign in and approve the connection. You can disconnect it anytime in Connected apps.
  discovery: https://www.creatorscompanion.app/.well-known/oauth-protected-resource
  discovery_http_status: 200
  name: MCP OAuth
  type: oauth2
slug: creatorscompanion-app-authentication
source_filename: creatorscompanion-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.creatorscompanion.app/connect\ndocs: https://www.creatorscompanion.app/connect\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  description: Remote MCP over HTTP with OAuth. The first time you use it, your AI app opens a CreatorsCompanion page where you sign in and approve the connection. You can disconnect it anytime in Connected apps.\n  applies_to: https://www.creatorscompanion.app/mcp\n  bearer_methods_supported:\n  - header\n  authorization_servers:\n  - https://loepapuzvunejbjoxixw.supabase.co/auth/v1\n  discovery: https://www.creatorscompanion.app/.well-known/oauth-protected-resource\n  discovery_http_status: 200\nnotes:\n- The protected-resource metadata (RFC 9728) was read by GET; no auth endpoints were called.\n- 'Docs: \"My AI app shows a 401 or unauthorized error. The connection was disconnected or its sign-in expired.\"'\n- A connected app can never buy credits, change your plan or billing, or act as\
  \ an admin.\n"
source_yaml_url: https://artifacts.apis.io/creatorscompanion-app/authentication/creatorscompanion-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Content Creation
- Creator Economy
- Social Media
- Artificial Intelligence
- Copywriting
- MCP
---
