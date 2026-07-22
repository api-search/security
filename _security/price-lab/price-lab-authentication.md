---
api_key_in: []
api_specs:
- filename: price-lab-openapi.yml
  format: yaml
  label: Price Lab API
  slug: price-lab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/price-lab/refs/heads/main/openapi/price-lab-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Price Lab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Price Lab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Price Lab
provider_slug: price-lab
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT access token obtained via POST /login/ and refreshed via POST /token/refresh/
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/price-lab-openapi.yml
  type: http
slug: price-lab-authentication
source_filename: price-lab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/price-lab-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token obtained via POST /login/ and refreshed via POST /token/refresh/\n  sources:\n  - openapi/price-lab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/price-lab/refs/heads/main/authentication/price-lab-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Pricing
- Retail
- E-commerce
- Competitive Intelligence
- Price Optimization
- Artificial Intelligence
- Electronic Shelf Labels
- Latin America
---
