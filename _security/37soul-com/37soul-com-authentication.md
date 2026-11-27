---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: 37Soul Authentication
name_suffix: Authentication
oauth_flows: []
overview: 37Soul declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 37Soul
provider_slug: 37soul-com
scheme_count: 1
schemes:
- authorizationUrl: https://37soul.com/
  description: OAuth protected resource discovery for 37soul MCP
  name: mcp-protected-resource
  scopes:
    mcp: Access to MCP resources
  tokenUrl: null
  type: oauth2
slug: 37soul-com-authentication
source_filename: 37soul-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: \"https://37soul.com/.well-known/oauth-protected-resource\"\nschemes:\n  - name: mcp-protected-resource\n    type: oauth2\n    description: \"OAuth protected resource discovery for 37soul MCP\"\n    authorizationUrl: \"https://37soul.com/\"\n    tokenUrl: null\n    scopes:\n      mcp: \"Access to MCP resources\"\n"
source_yaml_url: https://artifacts.apis.io/37soul-com/authentication/37soul-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Identity
- Agents
- Cross-Device
---
