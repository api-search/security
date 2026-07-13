---
api_key_in: []
api_specs:
- filename: clover-platform-rest-api-openapi.yml
  format: yaml
  label: Clover REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-platform-rest-api-openapi.yml
- filename: clover-ecommerce-api-openapi.yml
  format: yaml
  label: Clover Ecommerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-ecommerce-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Clover Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clover secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clover
provider_slug: clover
scheme_count: 2
schemes:
- description: OAuth 2.0 token or Ecommerce (PAKMS) API key.
  flows:
  - authorizationUrl: https://www.clover.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.clover.com/oauth/token
  name: OAuth2
  sources:
  - openapi/clover-ecommerce-api-openapi.yml
  type: oauth2
- description: OAuth 2.0 access token or merchant API token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clover-platform-rest-api-openapi.yml
  type: http
slug: clover-authentication
source_filename: clover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clover-ecommerce-api-openapi.yml, openapi/clover-platform-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.clover.com/oauth/authorize\n    tokenUrl: https://api.clover.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 token or Ecommerce (PAKMS) API key.\n  sources:\n  - openapi/clover-ecommerce-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token or merchant API token.\n  sources:\n  - openapi/clover-platform-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/authentication/clover-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Restaurant
- POS
- Payments
- Retail
- SMB
- Hardware
---
