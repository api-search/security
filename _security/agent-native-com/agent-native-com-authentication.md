---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agent-native-com-desktop-api-openapi.yml
  format: yaml
  label: agent-native-com Desktop API
  slug: agent-native-com-desktop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-native-com/openapi/agent-native-com-desktop-api-openapi.yml
- filename: agent-native-com-mcp-api-openapi.yml
  format: yaml
  label: agent-native-com MCP API
  slug: agent-native-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-native-com/openapi/agent-native-com-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agent Native Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: agent-native-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: agent-native-com
provider_slug: agent-native-com
scheme_count: 3
schemes:
- description: Magic link first authentication with email/password fallback and social providers.
  name: Better Auth Magic Link
  type: magic_link
- description: Standard OAuth 2.1 with PKCE for MCP hosts.
  flow: authorizationCode
  name: Remote MCP OAuth
  pkce: true
  type: oauth2
- description: Custom authentication via getSession callback (e.g., Clerk, Auth0, Firebase).
  name: Custom Session Callback
  type: custom
slug: agent-native-com-authentication
source_filename: agent-native-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://www.agent-native.com/docs/authentication.md\nschemes:\n  - type: magic_link\n    name: Better Auth Magic Link\n    description: Magic link first authentication with email/password fallback and social providers.\n  - type: oauth2\n    name: Remote MCP OAuth\n    flow: authorizationCode\n    pkce: true\n    description: Standard OAuth 2.1 with PKCE for MCP hosts.\n  - type: custom\n    name: Custom Session Callback\n    description: Custom authentication via getSession callback (e.g., Clerk, Auth0, Firebase).\n"
source_yaml_url: https://artifacts.apis.io/agent-native-com/authentication/agent-native-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI
- Agentic
- Framework
- Open-source
- DeveloperTools
---
