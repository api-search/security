---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bolt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bolt secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bolt
provider_slug: bolt
scheme_count: 2
schemes:
- in: header
  name: api-key
  parameter: X-API-Key
  sources:
  - openapi/bolt-api-reference-openapi.yaml
  type: apiKey
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: /v1/oauth/token
  name: oauth
  sources:
  - openapi/bolt-api-reference-openapi.yaml
  type: oauth2
slug: bolt-authentication
source_filename: bolt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bolt-api-reference-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/bolt-api-reference-openapi.yaml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\n    scopes: 3\n  sources:\n  - openapi/bolt-api-reference-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt/refs/heads/main/authentication/bolt-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Checkout
- Payments
- eCommerce
- One-Click Checkout
- Shopper Network
- Fraud Protection
---
