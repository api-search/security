---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for 3D Print Log REST API and MCP server.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: 3Dprintlog Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3D Print Log declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 3D Print Log
provider_slug: 3dprintlog-com
scheme_count: 3
schemes:
- evidence: 'Send it in the X-Api-Key header: curl -H "X-Api-Key: YOUR_API_KEY" https://api.3dprintlog.com/api/Users/me'
  header: X-Api-Key
  how_to_obtain: Create a personal API key on the Personal API Keys page; the key is shown once after creation.
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: An api_key query parameter also works, as a fallback for clients that can't set headers
  how_to_obtain: Same as above – use the personal API key created by the user.
  location: query
  name: api_key
  type: apiKey
- authorize_url: https://3dprintlog.auth0.com/authorize
  evidence: 'OAuth 2.0 access token Authorization: Bearer <token> header'
  flows:
  - authorization_code
  how_to_obtain: Use the published public client ID (uzxvtpefYIrWoYbaJteoRzZtIYw4wP7j) with the authorization code flow + PKCE; request the token from https://3dprintlog.auth0.com/oauth/token with the appropriate audience (https://api.3dprintlog.com/mcp for MCP or https://3dprintlog.com/api for REST).
  name: OAuth 2.0
  scopes:
  - read:printdata
  - write:printdata
  type: oauth2
slug: 3dprintlog-com-authentication
source_filename: 3dprintlog-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.3dprintlog.com/docs/api
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.3dprintlog.com/docs/api\nsources:\n- https://www.3dprintlog.com/docs/api\n- https://www.3dprintlog.com/auth.md\n- https://www.3dprintlog.com/docs/getting-started\ndescription: Authentication methods for 3D Print Log REST API and MCP server.\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'Send it in the X-Api-Key header: curl -H \"X-Api-Key: YOUR_API_KEY\" https://api.3dprintlog.com/api/Users/me'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create a personal API key on the Personal API Keys page; the key is shown once after creation.\n- type: apiKey\n  name: api_key\n  evidence: An api_key query parameter also works, as a fallback for clients that can't set headers\n  location: query\n  how_to_obtain: Same as above – use the personal API key created by the user.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'OAuth 2.0 access token Authorization:\
  \ Bearer <token> header'\n  flows:\n  - authorization_code\n  authorize_url: https://3dprintlog.auth0.com/authorize\n  scopes:\n  - read:printdata\n  - write:printdata\n  how_to_obtain: Use the published public client ID (uzxvtpefYIrWoYbaJteoRzZtIYw4wP7j) with the authorization code flow + PKCE; request the token\n    from https://3dprintlog.auth0.com/oauth/token with the appropriate audience (https://api.3dprintlog.com/mcp for MCP or https://3dprintlog.com/api\n    for REST).\ndocs: https://www.3dprintlog.com/docs/api\n"
source_yaml_url: https://artifacts.apis.io/3dprintlog-com/authentication/3dprintlog-com-authentication.yml
summary_line: 3 schemes
tags:
- 3D Printing
- Software-as-a-Service
- Analytics
- Inventory
- Community
---
