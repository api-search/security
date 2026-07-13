---
api_key_in:
- header
api_specs:
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Negotiated Rates
  slug: negotiated-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Rate Search
  slug: rate-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Datasets
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Benchmarks
  slug: benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Payerset Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payerset secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Payerset
provider_slug: payerset
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/payerset-openapi.yml
  type: apiKey
slug: payerset-authentication
source_filename: payerset-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/payerset-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/payerset-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/authentication/payerset-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Price Transparency
- Negotiated Rates
- Machine-Readable Files
- Payer Data
---
