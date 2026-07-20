---
api_key_in:
- header
api_specs:
- filename: deliverart-openapi.yml
  format: yaml
  label: Deliverart API
  slug: deliverart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Deliverart Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Deliverart secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Deliverart
provider_slug: deliverart
scheme_count: 2
schemes:
- description: API key issued by the Deliverart team, sent in the X-Deliverart-ApiKey header.
  in: header
  name: apiKey
  parameter: X-Deliverart-ApiKey
  sources:
  - openapi/deliverart-openapi.yml
  type: apiKey
- description: OAuth2 password grant. Token endpoint is on the auth host.
  flows:
  - flow: password
    scopes: 44
    tokenUrl: https://auth.deliverart.it/oauth
  name: oauth2
  sources:
  - openapi/deliverart-openapi.yml
  type: oauth2
slug: deliverart-authentication
source_filename: deliverart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/deliverart-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Deliverart-ApiKey\n  description: API key issued by the Deliverart team, sent in the X-Deliverart-ApiKey header.\n  sources:\n  - openapi/deliverart-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://auth.deliverart.it/oauth\n    scopes: 44\n  description: OAuth2 password grant. Token endpoint is on the auth host.\n  sources:\n  - openapi/deliverart-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/authentication/deliverart-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Food Delivery
- Restaurants
- Order Management
- Logistics
- Delivery
- Menu Management
- Point of Sale
---
