---
api_key_in: []
api_specs:
- filename: obol-address-api-openapi.yml
  format: yaml
  label: Obol Address API
  slug: obol-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-address-api-openapi.yml
- filename: obol-cluster-definition-api-openapi.yml
  format: yaml
  label: Obol Cluster Definition API
  slug: obol-cluster-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-cluster-definition-api-openapi.yml
- filename: obol-cluster-effectiveness-api-openapi.yml
  format: yaml
  label: Obol Cluster Effectiveness API
  slug: obol-cluster-effectiveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-cluster-effectiveness-api-openapi.yml
- filename: obol-cluster-lock-api-openapi.yml
  format: yaml
  label: Obol Cluster Lock API
  slug: obol-cluster-lock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-cluster-lock-api-openapi.yml
- filename: obol-deposit-data-api-openapi.yml
  format: yaml
  label: Obol Deposit Data API
  slug: obol-deposit-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-deposit-data-api-openapi.yml
- filename: obol-dv-exit-api-openapi.yml
  format: yaml
  label: Obol DV Exit API
  slug: obol-dv-exit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-dv-exit-api-openapi.yml
- filename: obol-dv-migrate-api-openapi.yml
  format: yaml
  label: Obol DV Migrate API
  slug: obol-dv-migrate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-dv-migrate-api-openapi.yml
- filename: obol-fee-recipient-api-openapi.yml
  format: yaml
  label: Obol Fee Recipient API
  slug: obol-fee-recipient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-fee-recipient-api-openapi.yml
- filename: obol-metrics-api-openapi.yml
  format: yaml
  label: Obol Metrics API
  slug: obol-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-metrics-api-openapi.yml
- filename: obol-owr-information-api-openapi.yml
  format: yaml
  label: Obol OWR Information API
  slug: obol-owr-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-owr-information-api-openapi.yml
- filename: obol-positions-api-openapi.yml
  format: yaml
  label: Obol Positions API
  slug: obol-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-positions-api-openapi.yml
- filename: obol-state-api-openapi.yml
  format: yaml
  label: Obol State API
  slug: obol-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-state-api-openapi.yml
- filename: obol-system-api-openapi.yml
  format: yaml
  label: Obol System API
  slug: obol-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-system-api-openapi.yml
- filename: obol-techne-credentials-api-openapi.yml
  format: yaml
  label: Obol Techne Credentials API
  slug: obol-techne-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-techne-credentials-api-openapi.yml
- filename: obol-terms-and-conditions-api-openapi.yml
  format: yaml
  label: Obol Terms And Conditions API
  slug: obol-terms-and-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-terms-and-conditions-api-openapi.yml
- filename: obol-test-api-openapi.yml
  format: yaml
  label: Obol Test API
  slug: obol-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-test-api-openapi.yml
- filename: obol-tvs-api-openapi.yml
  format: yaml
  label: Obol tvs API
  slug: obol-tvs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-tvs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Obol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Obol
provider_slug: obol
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/obol-openapi-original.json
  type: http
slug: obol-authentication
source_filename: obol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/obol-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/obol-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/authentication/obol-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto
- Ethereum
- Staking
- Distributed Validators
- Blockchain Infrastructure
- Web3
---
