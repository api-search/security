---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wego-countries-api-openapi.yml
  format: yaml
  label: Wego Countries API
  slug: wego-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-countries-api-openapi.yml
- filename: wego-feedback-api-openapi.yml
  format: yaml
  label: Wego Feedback API
  slug: wego-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-feedback-api-openapi.yml
- filename: wego-flights-api-openapi.yml
  format: yaml
  label: Wego Flights API
  slug: wego-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-flights-api-openapi.yml
- filename: wego-health-api-openapi.yml
  format: yaml
  label: Wego Health API
  slug: wego-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-health-api-openapi.yml
- filename: wego-hotels-api-openapi.yml
  format: yaml
  label: Wego Hotels API
  slug: wego-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-hotels-api-openapi.yml
- filename: wego-places-api-openapi.yml
  format: yaml
  label: Wego Places API
  slug: wego-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-places-api-openapi.yml
- filename: wego-user-api-openapi.yml
  format: yaml
  label: Wego User API
  slug: wego-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-user-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Wego Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wego secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wego
provider_slug: wego
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Wego auth server access token, sent as `Authorization: Bearer <token>` (RFC 6750).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wego-api-openapi.json
  type: http
- description: OAuth2 authorization-code flow (PKCE supported) against the Wego auth server.
  flows:
  - authorizationUrl: https://auth.wego.com/user-auth/v2/users/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.wego.com/user-auth/v2/users/oauth/token
  name: oauth2
  sources:
  - openapi/wego-api-openapi.json
  type: oauth2
slug: wego-authentication
source_filename: wego-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/wego-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Wego auth server access token, sent as `Authorization: Bearer <token>` (RFC\n    6750).'\n  sources:\n  - openapi/wego-api-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wego.com/user-auth/v2/users/oauth/authorize\n    tokenUrl: https://auth.wego.com/user-auth/v2/users/oauth/token\n    scopes: 3\n  description: OAuth2 authorization-code flow (PKCE supported) against the Wego auth server.\n  sources:\n  - openapi/wego-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/authentication/wego-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Travel
- Flights
- Hotels
- Metasearch
- Booking
- Agent-Native
- Tourism
- Search
---
