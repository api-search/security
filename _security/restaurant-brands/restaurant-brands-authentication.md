---
api_key_in: []
api_specs:
- filename: restaurant-brands-loyalty-api-openapi.yml
  format: yaml
  label: Restaurant Brands International Loyalty API
  slug: restaurant-brands-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/openapi/restaurant-brands-loyalty-api-openapi.yml
- filename: restaurant-brands-menus-api-openapi.yml
  format: yaml
  label: Restaurant Brands International Menus API
  slug: restaurant-brands-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/openapi/restaurant-brands-menus-api-openapi.yml
- filename: restaurant-brands-orders-api-openapi.yml
  format: yaml
  label: Restaurant Brands International Orders API
  slug: restaurant-brands-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/openapi/restaurant-brands-orders-api-openapi.yml
- filename: restaurant-brands-stores-api-openapi.yml
  format: yaml
  label: Restaurant Brands International Stores API
  slug: restaurant-brands-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/openapi/restaurant-brands-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Restaurant Brands Authentication
name_suffix: Authentication
oauth_flows: []
overview: Restaurant Brands International secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Restaurant Brands International
provider_slug: restaurant-brands
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/channel-openapi.yml
  - openapi/menu-v2-openapi.yml
  type: http
slug: restaurant-brands-authentication
source_filename: restaurant-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/channel-openapi.yml, openapi/menu-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/channel-openapi.yml\n  - openapi/menu-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/authentication/restaurant-brands-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 500
- Franchising
- Hospitality
- NYSE QSR
- Quick Service Restaurants
- Restaurant
---
