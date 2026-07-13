---
api_key_in:
- header
api_specs:
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Eligibility & Coverage API
  slug: eligibility-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Coverage Scan API
  slug: coverage-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Benefits API
  slug: benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Cost Estimation API
  slug: cost-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Medicaid API
  slug: medicaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nirvana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nirvana Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nirvana Health
provider_slug: nirvana
scheme_count: 1
schemes:
- description: Nirvana issues an API key on request. Pass it in the `apikey` request header on every call. Contact Nirvana to provision a key.
  in: header
  name: apiKeyHeader
  parameter: apikey
  sources:
  - openapi/nirvana-openapi.yml
  type: apiKey
slug: nirvana-authentication
source_filename: nirvana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nirvana-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Nirvana issues an API key on request. Pass it in the `apikey` request header\n    on every call. Contact Nirvana to provision a key.\n  sources:\n  - openapi/nirvana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/authentication/nirvana-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Insurance
- Eligibility
- Benefits
- Cost Estimation
- Behavioral Health
---
