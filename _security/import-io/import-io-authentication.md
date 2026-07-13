---
api_key_in:
- query
api_specs:
- filename: import-io-openapi.yml
  format: yaml
  label: Import.io API
  slug: import-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/import-io/main/openapi/import-io-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Import Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Import.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Import.io
provider_slug: import-io
scheme_count: 1
schemes:
- description: API key obtained from the Import.io dashboard User Settings.
  in: query
  name: apiKeyAuth
  parameter: _apikey
  sources:
  - openapi/import-io-openapi.yml
  type: apiKey
slug: import-io-authentication
source_filename: import-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/import-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: _apikey\n  description: API key obtained from the Import.io dashboard User Settings.\n  sources:\n  - openapi/import-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/import-io/refs/heads/main/authentication/import-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Aggregation
- Data Extraction
- Data Integration
- Pricing Intelligence
- Web Scraping
---
