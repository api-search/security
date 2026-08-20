---
api_key_in: []
api_specs:
- filename: veli-orders-api-openapi.yml
  format: yaml
  label: Veli Orders API
  slug: veli-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-orders-api-openapi.yml
- filename: veli-performance-api-openapi.yml
  format: yaml
  label: Veli Performance API
  slug: veli-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-performance-api-openapi.yml
- filename: veli-portfolios-api-openapi.yml
  format: yaml
  label: Veli Portfolios API
  slug: veli-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-portfolios-api-openapi.yml
- filename: veli-positions-api-openapi.yml
  format: yaml
  label: Veli Positions API
  slug: veli-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-positions-api-openapi.yml
- filename: veli-strategies-api-openapi.yml
  format: yaml
  label: Veli Strategies API
  slug: veli-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-strategies-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veli secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veli
provider_slug: veli
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT Bearer token for API authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/veli-openapi.yml
  type: http
slug: veli-authentication
source_filename: veli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veli-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token for API authentication\n  sources:\n  - openapi/veli-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/authentication/veli-authentication.yml
summary_line: http · 1 scheme
tags:
- Crypto
- DeFi
- Finance
- Investment
- Portfolio-Management
---
