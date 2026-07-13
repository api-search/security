---
api_key_in: []
api_specs:
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Account API
  slug: teelaunch-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Blank Catalog API
  slug: teelaunch-blank-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Products API
  slug: teelaunch-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Orders API
  slug: teelaunch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Shipping & Tracking API
  slug: teelaunch-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Platforms & Stores API
  slug: teelaunch-platforms-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teelaunch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teelaunch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teelaunch
provider_slug: teelaunch
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teelaunch-openapi.yml
  type: http
slug: teelaunch-authentication
source_filename: teelaunch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teelaunch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/teelaunch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/authentication/teelaunch-authentication.yml
summary_line: http · 1 scheme
tags:
- Print on Demand
- POD
- Ecommerce
- Fulfillment
- Dropshipping
- Orders
- Shipping
---
