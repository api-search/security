---
api_key_in: []
api_specs:
- filename: bitfinder-awair-openapi.yml
  format: yaml
  label: Awair Home & OAuth Developer API
  slug: awair-home-oauth-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitfinder/refs/heads/main/openapi/bitfinder-awair-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bitfinder Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bitfinder secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bitfinder
provider_slug: bitfinder
scheme_count: 2
schemes:
- description: Awair Developer Console access token or OAuth 2.0 access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bitfinder-awair-openapi.yml
  type: http
- description: OAuth 2.0 authorization-code flow for third-party access to Awair user data.
  flows:
  - authorizationUrl: https://oauth2.awair.is/v2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://oauth2.awair.is/v2/token
  name: oauth2
  sources:
  - openapi/bitfinder-awair-openapi.yml
  type: oauth2
slug: bitfinder-authentication
source_filename: bitfinder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bitfinder-awair-openapi.yml\ndocs: https://docs.developer.getawair.com/\nnotes: >-\n  Requests authenticate with an HTTP Bearer token in the Authorization header.\n  The token is either a Developer Console access token (obtained from the Awair\n  Developer Console, https://developer.getawair.com/) or an OAuth 2.0 access\n  token issued via the authorization-code flow for third-party apps acting on\n  behalf of Awair users. OAuth token exchange endpoint is\n  https://oauth2.awair.is/v2/token; refresh tokens are long-lived and access\n  tokens are short-lived.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Awair Developer Console access token or OAuth 2.0 access token.\n  sources:\n  - openapi/bitfinder-awair-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://oauth2.awair.is/v2/authorize\n    tokenUrl: https://oauth2.awair.is/v2/token\n    scopes: 0\n  description: OAuth 2.0 authorization-code flow for third-party access to Awair user data.\n  sources:\n  - openapi/bitfinder-awair-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfinder/refs/heads/main/authentication/bitfinder-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Air Quality
- Internet of Things
- IoT
- Environmental Monitoring
- Smart Home
- Sensors
- Health
- Developer API
---
