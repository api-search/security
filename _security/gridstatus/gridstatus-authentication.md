---
api_key_in:
- header
- query
api_specs:
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Datasets API
  slug: gridstatus-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Dataset Query API
  slug: gridstatus-dataset-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Pricing Locations API
  slug: gridstatus-pricing-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Constraints API
  slug: gridstatus-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Reports and Block Pricing API
  slug: gridstatus-reports-block-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Bulk Exports and Usage API
  slug: gridstatus-bulk-exports-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gridstatus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grid Status secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Grid Status
provider_slug: gridstatus
scheme_count: 2
schemes:
- description: API key from https://www.gridstatus.io/settings/api.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/gridstatus-openapi.yml
  type: apiKey
- description: API key passed as a query parameter (alternative to the header).
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/gridstatus-openapi.yml
  type: apiKey
slug: gridstatus-authentication
source_filename: gridstatus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gridstatus-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key from https://www.gridstatus.io/settings/api.\n  sources:\n  - openapi/gridstatus-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter (alternative to the header).\n  sources:\n  - openapi/gridstatus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/authentication/gridstatus-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Day-Ahead Prices
- Electricity
- Grid Data
- Energy Markets
- LMP
- Load
- Fuel Mix
- Open Source
---
