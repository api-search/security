---
api_key_in:
- header
- query
api_specs:
- filename: gridstatus-api-info-api-openapi.yml
  format: yaml
  label: Grid Status API Info API
  slug: gridstatus-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-api-info-api-openapi.yml
- filename: gridstatus-api-usage-api-openapi.yml
  format: yaml
  label: Grid Status API Usage API
  slug: gridstatus-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-api-usage-api-openapi.yml
- filename: gridstatus-block-pricing-data-api-openapi.yml
  format: yaml
  label: Grid Status Block Pricing Data API
  slug: gridstatus-block-pricing-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-block-pricing-data-api-openapi.yml
- filename: gridstatus-constraints-api-openapi.yml
  format: yaml
  label: Grid Status Constraints API
  slug: gridstatus-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-constraints-api-openapi.yml
- filename: gridstatus-csv-exports-api-openapi.yml
  format: yaml
  label: Grid Status CSV Exports API
  slug: gridstatus-csv-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-csv-exports-api-openapi.yml
- filename: gridstatus-dataset-audit-api-openapi.yml
  format: yaml
  label: Grid Status Dataset Audit API
  slug: gridstatus-dataset-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-dataset-audit-api-openapi.yml
- filename: gridstatus-dataset-metadata-api-openapi.yml
  format: yaml
  label: Grid Status Dataset Metadata API
  slug: gridstatus-dataset-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-dataset-metadata-api-openapi.yml
- filename: gridstatus-dataset-updates-api-openapi.yml
  format: yaml
  label: Grid Status Dataset Updates API
  slug: gridstatus-dataset-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-dataset-updates-api-openapi.yml
- filename: gridstatus-pricing-locations-api-openapi.yml
  format: yaml
  label: Grid Status Pricing Locations API
  slug: gridstatus-pricing-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-pricing-locations-api-openapi.yml
- filename: gridstatus-query-data-api-openapi.yml
  format: yaml
  label: Grid Status Query Data API
  slug: gridstatus-query-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-query-data-api-openapi.yml
- filename: gridstatus-reports-api-openapi.yml
  format: yaml
  label: Grid Status Reports API
  slug: gridstatus-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-reports-api-openapi.yml
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
