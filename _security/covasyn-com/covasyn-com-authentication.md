---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CovaSyn Authentication
name_suffix: Authentication
oauth_flows: []
overview: CovaSyn declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CovaSyn
provider_slug: covasyn-com
scheme_count: 3
schemes:
- description: API key generated in the CovaSyn dashboard under API keys; "It is shown only once, so copy it straight into your client configuration. Compromised keys can be revoked there at any time."
  in: header
  name: X-CovaSyn-Key
  type: apiKey
- description: 'The same API key sent as "Authorization: Bearer <your-key>" (documented as equivalent to X-CovaSyn-Key).'
  scheme: bearer
  type: http
- description: OAuth 2.1 with PKCE and dynamic client registration, used by MCP clients (Claude, ChatGPT) without manual key entry.
  discovery:
  - status: 200
    url: https://mcp.covasyn.com/.well-known/oauth-protected-resource
  - status: 200
    url: https://mcp.covasyn.com/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.covasyn.com/oauth/authorize
      pkce: S256
      registrationUrl: https://mcp.covasyn.com/oauth/register
      scopes:
      - mcp.tools.call
      - mcp.tools.list
      tokenUrl: https://mcp.covasyn.com/oauth/token
      token_endpoint_auth_methods:
      - none
  type: oauth2
slug: covasyn-com-authentication
source_filename: covasyn-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://covasyn.com/en/software/docs/mcp/auth\ndocs: https://covasyn.com/en/software/docs/mcp/auth\nschemes:\n- type: apiKey\n  in: header\n  name: X-CovaSyn-Key\n  description: API key generated in the CovaSyn dashboard under API keys; \"It is shown only once, so copy it straight into your client configuration. Compromised keys can be revoked there at any time.\"\n- type: http\n  scheme: bearer\n  description: 'The same API key sent as \"Authorization: Bearer <your-key>\" (documented as equivalent to X-CovaSyn-Key).'\n- type: oauth2\n  description: OAuth 2.1 with PKCE and dynamic client registration, used by MCP clients (Claude, ChatGPT) without manual key entry.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.covasyn.com/oauth/authorize\n      tokenUrl: https://mcp.covasyn.com/oauth/token\n      registrationUrl: https://mcp.covasyn.com/oauth/register\n      pkce: S256\n      token_endpoint_auth_methods:\
  \ [none]\n      scopes: [mcp.tools.call, mcp.tools.list]\n  discovery:\n  - url: https://mcp.covasyn.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://mcp.covasyn.com/.well-known/oauth-authorization-server\n    status: 200\nnote: Endpoints read from the documented discovery documents (GET only); the authorize/token/register endpoints were not called.\n"
source_yaml_url: https://artifacts.apis.io/covasyn-com/authentication/covasyn-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Chemistry
- Pharma
- Biotechnology
- Cheminformatics
- MCP
- Artificial Intelligence
- Quality and Regulatory
---
