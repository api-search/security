---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jobctl App Authentication
name_suffix: Authentication
oauth_flows: []
overview: jobctl-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: jobctl-app
provider_slug: jobctl-app
scheme_count: 1
schemes:
- description: OAuth2 authorization server discovered via well-known endpoint.
  discovery: https://jobctl.app/.well-known/oauth-authorization-server
  flow: authorization_code
  notes: Clients can skip token by using OAuth discovery as noted in docs.
  type: oauth2
slug: jobctl-app-authentication
source_filename: jobctl-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://jobctl.app/docs/\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    discovery: https://jobctl.app/.well-known/oauth-authorization-server\n    description: OAuth2 authorization server discovered via well-known endpoint.\n    notes: Clients can skip token by using OAuth discovery as noted in docs."
source_yaml_url: https://artifacts.apis.io/jobctl-app/authentication/jobctl-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Job-Tracking
- Developer-Tools
- AI
- MCP
- Productivity
---
