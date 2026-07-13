---
api_key_in: []
api_specs:
- filename: bringg-delivery-hub-api-openapi.yml
  format: yaml
  label: Bringg Delivery Hub API
  slug: bringg-delivery-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/openapi/bringg-delivery-hub-api-openapi.yml
- filename: bringg-drivers-shifts-api-openapi.yml
  format: yaml
  label: Bringg Drivers And Shifts API
  slug: bringg-drivers-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/openapi/bringg-drivers-shifts-api-openapi.yml
- filename: bringg-fleet-partners-api-openapi.yml
  format: yaml
  label: Bringg Fleet Partners API
  slug: bringg-fleet-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/openapi/bringg-fleet-partners-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bringg Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bringg secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bringg
provider_slug: bringg
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials Grant. Exchange your client_id and client_secret

    for an access token via POST https://admin-api.bringg.com/oauth/token (or the

    regional equivalent), then send Authorization: Bearer <access_token>.'
  flows:
  - flow: clientCredentials
    scopes: 13
    tokenUrl: https://admin-api.bringg.com/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/bringg-delivery-hub-api-openapi.yml
  - openapi/bringg-drivers-shifts-api-openapi.yml
  - openapi/bringg-fleet-partners-api-openapi.yml
  type: oauth2
slug: bringg-authentication
source_filename: bringg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bringg-delivery-hub-api-openapi.yml, openapi/bringg-drivers-shifts-api-openapi.yml,\n  openapi/bringg-fleet-partners-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://admin-api.bringg.com/oauth/token\n    scopes: 13\n  description: |-\n    OAuth 2.0 Client Credentials Grant. Exchange your client_id and client_secret\n    for an access token via POST https://admin-api.bringg.com/oauth/token (or the\n    regional equivalent), then send Authorization: Bearer <access_token>.\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n  - openapi/bringg-fleet-partners-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/authentication/bringg-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Last-Mile Delivery
- Delivery Orchestration
- Fulfillment
- Logistics
- Retail
- Dispatch
- Routing
- Driver App
- Carrier Network
- Fleet Management
- Supply Chain
- E-commerce
- Same-Day Delivery
- Curbside Pickup
- Returns
---
