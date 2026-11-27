---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AlphaProve Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlphaProve declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AlphaProve
provider_slug: alphaprove-com
scheme_count: 1
schemes:
- authorize_url: https://alphaprove.com/api/v1/oauth/authorize
  evidence: '"grant_types_supported":["authorization_code","refresh_token"]'
  flows:
  - authorization_code
  - refresh_token
  name: OAuth2
  scopes:
  - alphaprove:paper
  - alphaprove:read
  - alphaprove:research
  type: oauth2
slug: alphaprove-com-authentication
source_filename: alphaprove-com-authentication.yml
source_heading: Authentication Profile
source_url: https://alphaprove.com/.well-known/oauth-protected-resource/api/v1/mcp
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://alphaprove.com/.well-known/oauth-protected-resource/api/v1/mcp\nsources:\n- https://alphaprove.com/.well-known/oauth-protected-resource/api/v1/mcp\n- https://alphaprove.com/.well-known/oauth-authorization-server/api/v1/oauth\n- https://alphaprove.com/mcp\n- https://alphaprove.com/docs/getting-started/\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"grant_types_supported\":[\"authorization_code\",\"refresh_token\"]'\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://alphaprove.com/api/v1/oauth/authorize\n  scopes:\n  - alphaprove:paper\n  - alphaprove:read\n  - alphaprove:research\ndocs: https://alphaprove.com/.well-known/oauth-protected-resource/api/v1/mcp\n"
source_yaml_url: https://artifacts.apis.io/alphaprove-com/authentication/alphaprove-com-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Backtesting
- Trading
- Artificial Intelligence
- Finance
---
