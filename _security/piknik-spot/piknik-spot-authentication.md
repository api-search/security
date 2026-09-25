---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: piknik-spot-openapi.yml
  format: yaml
  label: Piknik.Spot REST API
  slug: piknikspot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/piknik-spot/refs/heads/main/openapi/piknik-spot-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Piknik Spot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Piknik.Spot secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Piknik.Spot
provider_slug: piknik-spot
scheme_count: 3
schemes:
- description: Session-based authentication for web browsers
  in: cookie
  name: cookieAuth
  parameter: next-auth.session-token
  sources:
  - openapi/piknik-spot-openapi.yml
  type: apiKey
- description: OAuth 2.0 authentication for external applications and AI agents
  flows:
  - authorizationUrl: https://piknik.spot/api/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://piknik.spot/api/oauth/token
  name: oauth2
  sources:
  - openapi/piknik-spot-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: 'OAuth2 access token (JWT). Include in Authorization header as: Bearer {token}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/piknik-spot-openapi.yml
  type: http
slug: piknik-spot-authentication
source_filename: piknik-spot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/piknik-spot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: next-auth.session-token\n  description: Session-based authentication for web browsers\n  sources:\n  - openapi/piknik-spot-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://piknik.spot/api/oauth/authorize\n    tokenUrl: https://piknik.spot/api/oauth/token\n    scopes: 4\n  description: OAuth 2.0 authentication for external applications and AI agents\n  sources:\n  - openapi/piknik-spot-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 access token (JWT). Include in Authorization header as: Bearer {token}'\n  sources:\n  - openapi/piknik-spot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piknik-spot/refs/heads/main/authentication/piknik-spot-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Local Food
- Agriculture
- Farmers Markets
- Marketplace
- Event
- Job
- Recipes
- Geolocation
- Community
- Food Systems
- MCP
- A2A
- Agent-Native
- Ontario
- Canada
---
