---
api_key_in: []
api_specs:
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Orders / Market API
  slug: orders-market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Contracts API
  slug: contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Prices / Quote API
  slug: prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Clusters / Nodes API
  slug: clusters-nodes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Balance API
  slug: balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Inference API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sfcompute Authentication
name_suffix: Authentication
oauth_flows: []
overview: SF Compute secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SF Compute
provider_slug: sfcompute
scheme_count: 1
schemes:
- description: 'API token created with `sf tokens create`, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sfcompute-openapi.yml
  type: http
slug: sfcompute-authentication
source_filename: sfcompute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sfcompute-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token created with `sf tokens create`, sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/sfcompute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/authentication/sfcompute-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- Compute
- Marketplace
- H100
- Spot Pricing
---
