---
api_key_in: []
api_specs:
- filename: lightspeed-pos-retail-x-series-openapi.yml
  format: yaml
  label: Lightspeed Retail X-Series API (Vend)
  slug: retail-x-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/openapi/lightspeed-pos-retail-x-series-openapi.yml
- filename: lightspeed-pos-retail-r-series-openapi.yml
  format: yaml
  label: Lightspeed Retail R-Series API
  slug: retail-r-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/openapi/lightspeed-pos-retail-r-series-openapi.yml
- filename: lightspeed-pos-restaurant-k-series-openapi.yml
  format: yaml
  label: Lightspeed Restaurant K-Series API
  slug: restaurant-k-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/openapi/lightspeed-pos-restaurant-k-series-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lightspeed Pos Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lightspeed secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lightspeed
provider_slug: lightspeed-pos
scheme_count: 1
schemes:
- description: 'The Lightspeed Restaurant K-Series APIs support OAuth2 authentication using the [authorization code grant flow](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/).

    See our [Authorization Quick Start Guide](https://api-portal.lsk.lightspeed.app/quick-start/authentication/authorization-overview) for more details on how to authenticate.'
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml
  - openapi/lightspeed-pos-retail-r-series-openapi.yml
  - openapi/lightspeed-pos-retail-x-series-openapi.yml
  type: oauth2
slug: lightspeed-pos-authentication
source_filename: lightspeed-pos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightspeed-pos-restaurant-k-series-openapi.yml, openapi/lightspeed-pos-retail-r-series-openapi.yml,\n  openapi/lightspeed-pos-retail-x-series-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 8\n  description: |-\n    The Lightspeed Restaurant K-Series APIs support OAuth2 authentication using the [authorization code grant flow](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/).\n    See our [Authorization Quick Start Guide](https://api-portal.lsk.lightspeed.app/quick-start/authentication/authorization-overview) for more details on how to authenticate.\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n  - openapi/lightspeed-pos-retail-x-series-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/authentication/lightspeed-pos-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- POS
- Retail
- Restaurant
- Ecommerce
---
