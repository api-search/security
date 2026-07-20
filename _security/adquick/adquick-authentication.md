---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adquick Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AdQuick secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AdQuick
provider_slug: adquick
scheme_count: 2
schemes:
- applies_to: AdQuick Partner REST API (https://api.adquick.com)
  in: header
  name: PartnerToken
  parameter_name: X-PARTNER-TOKEN
  source: https://docs.adquick.com/
  type: apiKey
- applies_to: AdQuick MCP Server (https://www.adquick.com/mcp)
  flows:
  - authorizationUrl: https://www.adquick.com/mcp/oauth/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://www.adquick.com/mcp/oauth/register
    revocationUrl: https://www.adquick.com/mcp/oauth/revoke
    scope_count: 6
    tokenUrl: https://www.adquick.com/mcp/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  name: MCPOAuth2
  scheme: oauth2
  source: https://www.adquick.com/.well-known/oauth-authorization-server
  type: oauth2
slug: adquick-authentication
source_filename: adquick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.adquick.com/\ndocs: https://docs.adquick.com/\nnotes: >-\n  No first-party OpenAPI is published (docs are a Cloudflare-fronted docs site), so this profile is\n  searched from the developer documentation and the live OAuth discovery metadata rather than derived\n  from a spec. AdQuick has two distinct authentication surfaces: a partner REST API using a static\n  header token, and a hosted MCP server using OAuth 2.0 with PKCE.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: PartnerToken\n  type: apiKey\n  in: header\n  parameter_name: X-PARTNER-TOKEN\n  applies_to: AdQuick Partner REST API (https://api.adquick.com)\n  source: https://docs.adquick.com/\n- name: MCPOAuth2\n  type: oauth2\n  scheme: oauth2\n  applies_to: AdQuick MCP Server (https://www.adquick.com/mcp)\n  source: https://www.adquick.com/.well-known/oauth-authorization-server\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://www.adquick.com/mcp/oauth/authorize\n    tokenUrl: https://www.adquick.com/mcp/oauth/token\n    revocationUrl: https://www.adquick.com/mcp/oauth/revoke\n    registrationUrl: https://www.adquick.com/mcp/oauth/register\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_post]\n    dynamic_client_registration: true\n    scope_count: 6\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adquick/refs/heads/main/authentication/adquick-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Enterprise Saas
- Advertising
- Out Of Home Advertising
- DOOH
- Programmatic Advertising
- Media Buying
- Marketing
- MCP
---
