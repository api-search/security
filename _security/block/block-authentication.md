---
api_key_in: []
api_specs:
- filename: block-square-api-openapi.yaml
  format: yaml
  label: Square API
  slug: block-square-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/openapi/block-square-api-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Block Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Block secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Block
provider_slug: block
scheme_count: 2
schemes:
- description: Personal access token for Square API
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/block-square-api-openapi.yaml
  type: http
- flows:
  - authorizationUrl: https://connect.squareup.com/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://connect.squareup.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/block-square-api-openapi.yaml
  type: oauth2
slug: block-authentication
source_filename: block-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/block-square-api-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token for Square API\n  sources:\n  - openapi/block-square-api-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.squareup.com/oauth2/authorize\n    tokenUrl: https://connect.squareup.com/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/block-square-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/authentication/block-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
---
