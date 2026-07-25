---
api_key_in: []
api_specs:
- filename: circana-brands-api-openapi.yml
  format: yaml
  label: Circana Brands API
  slug: circana-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-brands-api-openapi.yml
- filename: circana-categories-api-openapi.yml
  format: yaml
  label: Circana Categories API
  slug: circana-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-categories-api-openapi.yml
- filename: circana-consumer-panel-api-openapi.yml
  format: yaml
  label: Circana Consumer Panel API
  slug: circana-consumer-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-consumer-panel-api-openapi.yml
- filename: circana-exports-api-openapi.yml
  format: yaml
  label: Circana Exports API
  slug: circana-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-exports-api-openapi.yml
- filename: circana-market-data-api-openapi.yml
  format: yaml
  label: Circana Market Data API
  slug: circana-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-market-data-api-openapi.yml
- filename: circana-reports-api-openapi.yml
  format: yaml
  label: Circana Reports API
  slug: circana-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-reports-api-openapi.yml
- filename: circana-retailers-api-openapi.yml
  format: yaml
  label: Circana Retailers API
  slug: circana-retailers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-retailers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circana
provider_slug: circana
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained through Circana authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/circana-liquid-data.yaml
  type: http
slug: circana-authentication
source_filename: circana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circana-liquid-data.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained through Circana authentication\n  sources:\n  - openapi/circana-liquid-data.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/authentication/circana-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
---
