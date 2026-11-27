---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: BankruptcyObserver Authentication
name_suffix: Authentication
oauth_flows: []
overview: BankruptcyObserver declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: BankruptcyObserver
provider_slug: bankruptcyobserver-com
scheme_count: 5
schemes:
- description: 'Send Authorization: Bearer <your token> on every request. Token available in dashboard after subscription.'
  scheme: bearer
  type: http
- description: Alternative header for token.
  in: header
  name: X-API-Key
  type: apiKey
- description: URL token query parameter form.
  in: query
  name: api_key
  type: apiKey
- description: URL token path form.
  in: path
  name: api_key
  type: apiKey
- description: OAuth 2.1 with DCR and PKCE S256.
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.bankruptcyobserver.com/oauth/authorize
      scopes: {}
      tokenUrl: https://mcp.bankruptcyobserver.com/oauth/token
  type: oauth2
slug: bankruptcyobserver-com-authentication
source_filename: bankruptcyobserver-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://mcp.bankruptcyobserver.com/docs\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Send Authorization: Bearer <your token> on every request. Token available in dashboard after subscription.\"\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: \"Alternative header for token.\"\n  - type: apiKey\n    in: query\n    name: api_key\n    description: \"URL token query parameter form.\"\n  - type: apiKey\n    in: path\n    name: api_key\n    description: \"URL token path form.\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://mcp.bankruptcyobserver.com/oauth/authorize\n        tokenUrl: https://mcp.bankruptcyobserver.com/oauth/token\n        scopes: {}\n    description: \"OAuth 2.1 with DCR and PKCE S256.\"\n"
source_yaml_url: https://artifacts.apis.io/bankruptcyobserver-com/authentication/bankruptcyobserver-com-authentication.yml
summary_line: 5 schemes
tags:
- Bankruptcy
- Finance
- Legal
- Alerts
- US
---
