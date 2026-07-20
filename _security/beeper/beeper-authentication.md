---
api_key_in: []
api_specs:
- filename: beeper-desktop-api-openapi-original.yml
  format: yaml
  label: Beeper Desktop API
  slug: beeper-desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-desktop-api-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Beeper Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Beeper secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Beeper
provider_slug: beeper
scheme_count: 2
schemes:
- description: Bearer token authentication. Access token obtained via OAuth2 PKCE flow or created in-app. Required for all API operations.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/beeper-desktop-api-openapi-original.yml
  type: http
- description: OAuth2 Authorization Code flow with PKCE for obtaining bearer access tokens. Used by MCP servers to authenticate clients.
  flows:
  - authorizationUrl: http://localhost:23373/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: http://localhost:23373/oauth/token
  name: oauth2
  sources:
  - openapi/beeper-desktop-api-openapi-original.yml
  type: oauth2
slug: beeper-authentication
source_filename: beeper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beeper-desktop-api-openapi-original.yml\ndocs: https://developers.beeper.com/desktop-api/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Access token obtained via OAuth2 PKCE flow or created\n    in-app. Required for all API operations.\n  sources:\n  - openapi/beeper-desktop-api-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: http://localhost:23373/oauth/authorize\n    tokenUrl: http://localhost:23373/oauth/token\n    scopes: 2\n  description: OAuth2 Authorization Code flow with PKCE for obtaining bearer access tokens.\n    Used by MCP servers to authenticate clients.\n  sources:\n  - openapi/beeper-desktop-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/authentication/beeper-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Messaging
- Chat
- Communication
- Matrix
- MCP
- Desktop
- Aggregator
---
