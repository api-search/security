---
api_key_in: []
api_specs:
- filename: uber-eats-openapi.yml
  format: yaml
  label: Uber Eats Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/openapi/uber-eats-openapi.yml
- filename: uber-direct-openapi.yml
  format: yaml
  label: Uber Direct (Deliveries) API
  slug: uber-direct
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/openapi/uber-direct-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Uber Eats Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Uber Eats secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Uber Eats
provider_slug: uber-eats
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://auth.uber.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/uber-direct-openapi.yml
  - openapi/uber-eats-openapi.yml
  type: oauth2
slug: uber-eats-authentication
source_filename: uber-eats-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uber-direct-openapi.yml, openapi/uber-eats-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.uber.com/oauth/v2/token\n    scopes: 1\n  sources:\n  - openapi/uber-direct-openapi.yml\n  - openapi/uber-eats-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/authentication/uber-eats-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Uber Eats
- Uber Direct
- Food Delivery
- Last-Mile Logistics
- Restaurants
- Menus
- Orders
- Fulfillment
- Courier
- OAuth2
---
