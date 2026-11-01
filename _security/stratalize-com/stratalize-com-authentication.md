---
anonymous_access: false
api_key_in: []
api_specs:
- filename: stratalize-com-x402-api-openapi.yml
  format: yaml
  label: stratalize-com X402 API
  slug: stratalize-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stratalize-com/openapi/stratalize-com-x402-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Stratalize Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: stratalize-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: stratalize-com
provider_slug: stratalize-com
scheme_count: 1
schemes:
- description: OAuth 2.0 Authorization Code flow with PKCE (RFC 7636)
  flows:
    authorizationCode:
      authorizationUrl: https://www.stratalize.com/api/mcp/oauth/authorize
      refreshUrl: https://www.stratalize.com/api/mcp/oauth/token
      scopes: {}
      tokenUrl: https://www.stratalize.com/api/mcp/oauth/token
  type: oauth2
slug: stratalize-com-authentication
source_filename: stratalize-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://www.stratalize.com/docs/mcp\nschemes:\n  - type: oauth2\n    description: OAuth 2.0 Authorization Code flow with PKCE (RFC 7636)\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.stratalize.com/api/mcp/oauth/authorize\n        tokenUrl: https://www.stratalize.com/api/mcp/oauth/token\n        refreshUrl: https://www.stratalize.com/api/mcp/oauth/token\n        scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/stratalize-com/authentication/stratalize-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Construction
- Project Controls
- Schedule Management
- AI
- Compliance
---
