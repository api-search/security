---
api_key_in:
- query
api_specs:
- filename: federal-communications-commission-datasets-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Datasets API
  slug: federal-communications-commission-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-datasets-api-openapi.yml
- filename: federal-communications-commission-filings-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Filings API
  slug: federal-communications-commission-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-filings-api-openapi.yml
- filename: federal-communications-commission-pirate-radio-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Pirate Radio API
  slug: federal-communications-commission-pirate-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-pirate-radio-api-openapi.yml
- filename: federal-communications-commission-proceedings-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Proceedings API
  slug: federal-communications-commission-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-proceedings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Federal Communications Commission Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Communications Commission secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Federal Communications Commission
provider_slug: federal-communications-commission
scheme_count: 1
schemes:
- description: api.data.gov API key passed as a query parameter.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/ecfs.yml
  type: apiKey
slug: federal-communications-commission-authentication
source_filename: federal-communications-commission-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ecfs.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: api.data.gov API key passed as a query parameter.\n  sources:\n  - openapi/ecfs.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/authentication/federal-communications-commission-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Communications
- Federal Government
- Open Data
---
