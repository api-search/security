---
api_key_in: []
api_specs:
- filename: sfcompute-account-api-openapi.yml
  format: yaml
  label: SF Compute Account API
  slug: sfcompute-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-account-api-openapi.yml
- filename: sfcompute-balance-api-openapi.yml
  format: yaml
  label: SF Compute Balance API
  slug: sfcompute-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-balance-api-openapi.yml
- filename: sfcompute-clusters-api-openapi.yml
  format: yaml
  label: SF Compute Clusters API
  slug: sfcompute-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-clusters-api-openapi.yml
- filename: sfcompute-contracts-api-openapi.yml
  format: yaml
  label: SF Compute Contracts API
  slug: sfcompute-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-contracts-api-openapi.yml
- filename: sfcompute-nodes-api-openapi.yml
  format: yaml
  label: SF Compute Nodes API
  slug: sfcompute-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-nodes-api-openapi.yml
- filename: sfcompute-orders-api-openapi.yml
  format: yaml
  label: SF Compute Orders API
  slug: sfcompute-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-orders-api-openapi.yml
- filename: sfcompute-prices-api-openapi.yml
  format: yaml
  label: SF Compute Prices API
  slug: sfcompute-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-prices-api-openapi.yml
- filename: sfcompute-images-api-openapi.yml
  format: yaml
  label: SF Compute Images API
  slug: sfcompute-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-images-api-openapi.yml
- filename: sfcompute-money-api-openapi.yml
  format: yaml
  label: SF Compute Money API
  slug: sfcompute-money-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-money-api-openapi.yml
- filename: sfcompute-vms-api-openapi.yml
  format: yaml
  label: SF Compute V Ms API
  slug: sfcompute-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-vms-api-openapi.yml
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
