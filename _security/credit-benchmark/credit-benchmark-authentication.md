---
api_key_in: []
api_specs:
- filename: credit-benchmark-consensus-data-openapi.yml
  format: yaml
  label: Credit Benchmark Consensus Data API
  slug: credit-benchmark-consensus-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credit-benchmark/refs/heads/main/openapi/credit-benchmark-consensus-data-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Credit Benchmark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credit Benchmark secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Credit Benchmark
provider_slug: credit-benchmark
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/credit-benchmark-consensus-data-openapi.yml
  type: http
slug: credit-benchmark-authentication
source_filename: credit-benchmark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/credit-benchmark-consensus-data-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token.\n  sources:\n  - openapi/credit-benchmark-consensus-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credit-benchmark/refs/heads/main/authentication/credit-benchmark-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Credit Risk
- Credit Ratings
- Financial Data
- Analytics
- Data
- API
---
