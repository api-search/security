---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compute-comparison-prices-api-openapi.yml
  format: yaml
  label: Compute Comparison Prices API
  slug: compute-comparison-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compute-comparison/openapi/compute-comparison-prices-api-openapi.yml
- filename: compute-comparison-status-api-openapi.yml
  format: yaml
  label: Compute Comparison Status API
  slug: compute-comparison-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compute-comparison/openapi/compute-comparison-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Compute Comparison Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compute Comparison declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Compute Comparison
provider_slug: compute-comparison
scheme_count: 2
schemes:
- description: Optional API key to unlock full price history.
  in: query
  name: api_key
  type: apiKey
- bearerFormat: JWT
  description: Optional Bearer token for full history access.
  scheme: bearer
  type: http
slug: compute-comparison-authentication
source_filename: compute-comparison-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://computecomparison.com/api-docs\nschemes:\n  - type: apiKey\n    name: api_key\n    in: query\n    description: Optional API key to unlock full price history.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Optional Bearer token for full history access.\n"
source_yaml_url: https://artifacts.apis.io/compute-comparison/authentication/compute-comparison-authentication.yml
summary_line: 2 schemes
tags:
- Company
- GPU
- LLM
- Cloud
- Pricing
- Comparison
---
