---
api_key_in: []
api_specs:
- filename: pulsoid-features-api-openapi.yml
  format: yaml
  label: Pulsoid Features API
  slug: pulsoid-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-features-api-openapi.yml
- filename: pulsoid-geometry-dash-api-openapi.yml
  format: yaml
  label: Pulsoid Geometry Dash API
  slug: pulsoid-geometry-dash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-geometry-dash-api-openapi.yml
- filename: pulsoid-heart-rate-api-openapi.yml
  format: yaml
  label: Pulsoid Heart Rate API
  slug: pulsoid-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-heart-rate-api-openapi.yml
- filename: pulsoid-oauth2-api-openapi.yml
  format: yaml
  label: Pulsoid OAuth2 API
  slug: pulsoid-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-oauth2-api-openapi.yml
- filename: pulsoid-profile-api-openapi.yml
  format: yaml
  label: Pulsoid Profile API
  slug: pulsoid-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-profile-api-openapi.yml
- filename: pulsoid-statistics-api-openapi.yml
  format: yaml
  label: Pulsoid Statistics API
  slug: pulsoid-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-statistics-api-openapi.yml
- filename: pulsoid-token-api-openapi.yml
  format: yaml
  label: Pulsoid Token API
  slug: pulsoid-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-token-api-openapi.yml
- filename: pulsoid-widgets-api-openapi.yml
  format: yaml
  label: Pulsoid Widgets API
  slug: pulsoid-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-widgets-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pulsoid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Pulsoid secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Pulsoid
provider_slug: pulsoid
scheme_count: 2
schemes:
- bearerFormat: OAuth2
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pulsoid-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://pulsoid.net/oauth2/authorize
    flow: implicit
    scopes: 9
  - authorizationUrl: https://pulsoid.net/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://pulsoid.net/oauth2/token
  name: OAuth2
  sources:
  - openapi/pulsoid-openapi.yml
  type: oauth2
slug: pulsoid-authentication
source_filename: pulsoid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pulsoid-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  sources:\n  - openapi/pulsoid-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://pulsoid.net/oauth2/authorize\n    scopes: 9\n  - flow: authorizationCode\n    authorizationUrl: https://pulsoid.net/oauth2/authorize\n    tokenUrl: https://pulsoid.net/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/pulsoid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/authentication/pulsoid-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Heart Rate
- Health
- Wearables
- Real-Time
- Streaming
- WebSocket
- Authentication
---
