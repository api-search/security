---
api_key_in: []
api_specs:
- filename: nas-academy-openapi-original.json
  format: json
  label: Nas.com Public Discovery API
  slug: nascom-public-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nas-academy/refs/heads/main/openapi/nas-academy-openapi-original.json
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nas Academy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nas.com (Nas Academy) secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nas.com (Nas Academy)
provider_slug: nas-academy
scheme_count: 2
schemes:
- applies_to: https://nas.com/openapi.json
  description: Public read-only discovery resources require no credentials.
  name: PublicDiscovery
  type: none
- applies_to: https://mcp.nas.com/mcp
  authorization_server: https://auth.nas.io
  flows:
  - authorizationUrl: https://auth.nas.com/oauth/authorize
    dynamic_client_registration: https://auth.nas.com/oauth/register
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.nas.com/oauth/token
  issuer: https://auth.nas.com
  name: OAuth2Bearer
  scheme: bearer
  scopes:
  - nas.communities.read
  - nas.communities.write
  - nas.members.read
  - nas.products.read
  - nas.products.write
  - nas.orders.read
  type: oauth2
slug: nas-academy-authentication
source_filename: nas-academy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nas.com/auth.md\ndocs: https://nas.com/auth.md\nsummary:\n  types: [none, oauth2]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Nas.com exposes public agent discovery (OpenAPI, llms.txt, well-known documents, page context)\n    as read-only, unauthenticated resources — the Public Discovery OpenAPI declares no security\n    schemes. The official hosted Nas.com MCP endpoint (https://mcp.nas.com/mcp) requires an OAuth\n    bearer token from https://auth.nas.io with the appropriate scopes.\nschemes:\n  - name: PublicDiscovery\n    type: none\n    applies_to: https://nas.com/openapi.json\n    description: Public read-only discovery resources require no credentials.\n  - name: OAuth2Bearer\n    type: oauth2\n    applies_to: https://mcp.nas.com/mcp\n    scheme: bearer\n    issuer: https://auth.nas.com\n    authorization_server: https://auth.nas.io\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://auth.nas.com/oauth/authorize\n        tokenUrl: https://auth.nas.com/oauth/token\n        pkce: S256\n        dynamic_client_registration: https://auth.nas.com/oauth/register\n    scopes:\n      - nas.communities.read\n      - nas.communities.write\n      - nas.members.read\n      - nas.products.read\n      - nas.products.write\n      - nas.orders.read\noauth_discovery_chain:\n  - https://nas.com/auth.md\n  - https://mcp.nas.com/.well-known/oauth-protected-resource\n  - https://auth.nas.io/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nas-academy/refs/heads/main/authentication/nas-academy-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Company
- Creator Economy
- Community
- E-commerce
- AI
- Agents
- MCP
- Online Courses
- Sellers
---
