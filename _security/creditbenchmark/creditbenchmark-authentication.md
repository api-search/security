---
api_key_in: []
api_specs:
- filename: creditbenchmark-openapi-original.yml
  format: yaml
  label: Credit Benchmark API
  slug: credit-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-openapi-original.yml
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
