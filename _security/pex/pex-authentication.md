---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pex Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pex secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pex
provider_slug: pex
scheme_count: 3
schemes:
- applies_to: Pex Discovery API
  docs: https://docs.api.pex.com/
  key_management: https://drm.pex.com/settings/api-keys
  location: 'Authorization: Bearer {API_KEY}'
  name: DiscoveryBearerApiKey
  notes: Static API key issued in the Pex DRM settings, presented as a bearer token on every request.
  scheme: bearer
  type: http
- applies_to:
  - Pex AI Song Detector API
  - Pex Search API
  flows:
  - client_auth: HTTP Basic (CLIENT_ID:CLIENT_SECRET)
    expires_in: 7200
    flow: clientCredentials
    grant_type: client_credentials
    tokenUrl: https://api.ae.pex.com/oauth2/token
    token_type: Bearer
  name: OAuth2ClientCredentials
  notes: Access tokens are valid for two hours (7200s) and should be reused across requests until expiry rather than re-minted per call.
  scopes: []
  type: oauth2
- applies_to: Vobile MCP (mcp.pex.com)
  flows:
  - authorizationUrl: https://mcp.pex.com/mcp/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://mcp.pex.com/mcp/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: MCPOAuth2
  notes: Authorization-code + refresh-token flow with PKCE (S256); advertised via /.well-known/oauth-authorization-server on mcp.pex.com.
  scopes: []
  type: oauth2
slug: pex-authentication
source_filename: pex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pex.com/ (Search, AI Song Detector, and Discovery API auth docs)\ndocs: https://docs.pex.com/search/api-documentation/authentication\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: DiscoveryBearerApiKey\n  type: http\n  scheme: bearer\n  applies_to: Pex Discovery API\n  location: 'Authorization: Bearer {API_KEY}'\n  key_management: https://drm.pex.com/settings/api-keys\n  docs: https://docs.api.pex.com/\n  notes: Static API key issued in the Pex DRM settings, presented as a bearer token on every request.\n- name: OAuth2ClientCredentials\n  type: oauth2\n  applies_to: [Pex AI Song Detector API, Pex Search API]\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ae.pex.com/oauth2/token\n    client_auth: HTTP Basic (CLIENT_ID:CLIENT_SECRET)\n    grant_type: client_credentials\n    token_type: Bearer\n    expires_in: 7200\n  scopes: []\n\
  \  notes: Access tokens are valid for two hours (7200s) and should be reused across requests until expiry rather than re-minted per call.\n- name: MCPOAuth2\n  type: oauth2\n  applies_to: Vobile MCP (mcp.pex.com)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.pex.com/mcp/oauth/authorize\n    tokenUrl: https://mcp.pex.com/mcp/oauth/token\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    pkce: [S256]\n  scopes: []\n  notes: Authorization-code + refresh-token flow with PKCE (S256); advertised via /.well-known/oauth-authorization-server on mcp.pex.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pex/refs/heads/main/authentication/pex-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Developer Tools
- Content Identification
- Digital Rights Management
- Music
- Audio Recognition
- Artificial Intelligence
- Content Recognition
- Media
- MCP
---
