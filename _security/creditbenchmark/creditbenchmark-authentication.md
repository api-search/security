---
api_key_in: []
api_specs:
- filename: creditbenchmark-analytics-api-openapi.yml
  format: yaml
  label: Credit Benchmark Analytics API
  slug: creditbenchmark-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-analytics-api-openapi.yml
- filename: creditbenchmark-authentication-api-openapi.yml
  format: yaml
  label: Credit Benchmark Authentication API
  slug: creditbenchmark-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-authentication-api-openapi.yml
- filename: creditbenchmark-contributor-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Contributor Data API
  slug: creditbenchmark-contributor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-contributor-data-api-openapi.yml
- filename: creditbenchmark-entity-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Data API
  slug: creditbenchmark-entity-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-data-api-openapi.yml
- filename: creditbenchmark-entity-matching-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Matching API
  slug: creditbenchmark-entity-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-matching-api-openapi.yml
- filename: creditbenchmark-portfolio-analytics-api-openapi.yml
  format: yaml
  label: Credit Benchmark Portfolio Analytics API
  slug: creditbenchmark-portfolio-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-portfolio-analytics-api-openapi.yml
- filename: creditbenchmark-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Data API
  slug: creditbenchmark-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-data-api-openapi.yml
- filename: creditbenchmark-entity-resolution-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Resolution API
  slug: creditbenchmark-entity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-resolution-api-openapi.yml
- filename: creditbenchmark-metadata-api-openapi.yml
  format: yaml
  label: Credit Benchmark Metadata API
  slug: creditbenchmark-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-metadata-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Creditbenchmark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credit Benchmark secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Credit Benchmark
provider_slug: creditbenchmark
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/creditbenchmark-openapi-original.yml
  type: http
slug: creditbenchmark-authentication
source_filename: creditbenchmark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/creditbenchmark-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token.\n  sources:\n  - openapi/creditbenchmark-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/authentication/creditbenchmark-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Credit Risk
- Financial Data
- Credit Ratings
- Analytics
- Risk Management
- Entity Resolution
- Consensus Data
---
