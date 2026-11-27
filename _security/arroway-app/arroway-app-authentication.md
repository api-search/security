---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arroway-app-mcp.json
  format: json
  label: Arroway MCP API
  slug: arroway-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arroway-app/openapi/arroway-app-mcp.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arroway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arroway declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Arroway
provider_slug: arroway-app
scheme_count: 1
schemes:
- flows:
    authorizationCode:
      authorizationUrl: https://www.arroway.app/oauth/authorize
      scopes:
        mcp: Access to MCP
      tokenUrl: https://www.arroway.app/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://www.arroway.app/oauth/device_authorization
      scopes:
        mcp: Access to MCP
      tokenUrl: https://www.arroway.app/oauth/token
    jwtBearer:
      scopes:
        mcp: Access to MCP
      tokenUrl: https://www.arroway.app/oauth/token
  type: oauth2
slug: arroway-app-authentication
source_filename: arroway-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://www.arroway.app/auth.md\nschemes:\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.arroway.app/oauth/authorize\n        tokenUrl: https://www.arroway.app/oauth/token\n        scopes:\n          mcp: \"Access to MCP\"\n      deviceCode:\n        deviceAuthorizationUrl: https://www.arroway.app/oauth/device_authorization\n        tokenUrl: https://www.arroway.app/oauth/token\n        scopes:\n          mcp: \"Access to MCP\"\n      jwtBearer:\n        tokenUrl: https://www.arroway.app/oauth/token\n        scopes:\n          mcp: \"Access to MCP\"\n"
source_yaml_url: https://artifacts.apis.io/arroway-app/authentication/arroway-app-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Collaboration
- Memory
- Teamwork
- Automation
---
