---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Powmcp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: powmcp-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: powmcp-com
provider_slug: powmcp-com
scheme_count: 1
schemes:
- flows:
    implicit:
      authorizationUrl: https://clerk.powmcp.com
      scopes:
        email: ''
        profile: ''
  type: oauth2
slug: powmcp-com-authentication
source_filename: powmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://powmcp.com/.well-known/oauth-protected-resource/website-speed-test/mcp\nschemes:\n  - type: oauth2\n    flows:\n      implicit:\n        authorizationUrl: https://clerk.powmcp.com\n        scopes:\n          profile: \"\"\n          email: \"\"\n"
source_yaml_url: https://artifacts.apis.io/powmcp-com/authentication/powmcp-com-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Utilities
- ChatGPT
- Claude
- MCP
---
