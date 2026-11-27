---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: 1Social Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Social declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 1Social
provider_slug: 1social-dev
scheme_count: 1
schemes:
- description: Bearer token required for MCP endpoint
  flow: client_credentials
  tokenUrl: https://mcp.1social.dev/.well-known/oauth-protected-resource
  type: oauth2
slug: 1social-dev-authentication
source_filename: 1social-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://mcp.1social.dev/mcp\nschemes:\n  - type: oauth2\n    flow: client_credentials\n    tokenUrl: https://mcp.1social.dev/.well-known/oauth-protected-resource\n    description: \"Bearer token required for MCP endpoint\"\n"
source_yaml_url: https://artifacts.apis.io/1social-dev/authentication/1social-dev-authentication.yml
summary_line: 1 scheme
tags:
- Social Media
- AI Integration
- Automation
- Content Publishing
- ChatGPT
---
