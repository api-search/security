---
api_key_in:
- header
api_specs:
- filename: clari-activity-api-api-openapi.yml
  format: yaml
  label: Clari Activity API API
  slug: clari-activity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-activity-api-api-openapi.yml
- filename: clari-administrative-api-api-openapi.yml
  format: yaml
  label: Clari Administrative API API
  slug: clari-administrative-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-administrative-api-api-openapi.yml
- filename: clari-audit-api-api-openapi.yml
  format: yaml
  label: Clari Audit API API
  slug: clari-audit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-audit-api-api-openapi.yml
- filename: clari-bulk-export-framework-api-openapi.yml
  format: yaml
  label: Clari Bulk Export Framework API
  slug: clari-bulk-export-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-export-framework-api-openapi.yml
- filename: clari-bulk-ingest-job-status-api-api-openapi.yml
  format: yaml
  label: Clari Bulk Ingest Job Status API API
  slug: clari-bulk-ingest-job-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-ingest-job-status-api-api-openapi.yml
- filename: clari-export-api-openapi.yml
  format: yaml
  label: Clari Export API
  slug: clari-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-export-api-openapi.yml
- filename: clari-forecast-api-api-openapi.yml
  format: yaml
  label: Clari Forecast API API
  slug: clari-forecast-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-forecast-api-api-openapi.yml
- filename: clari-ingestion-api-api-openapi.yml
  format: yaml
  label: Clari Ingestion API API
  slug: clari-ingestion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-ingestion-api-api-openapi.yml
- filename: clari-opportunity-api-api-openapi.yml
  format: yaml
  label: Clari Opportunity API API
  slug: clari-opportunity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-opportunity-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clari secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clari
provider_slug: clari
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: apikey
  sources:
  - openapi/clari-revenue-api-openapi.yml
  type: apiKey
slug: clari-authentication
source_filename: clari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clari-revenue-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/clari-revenue-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/authentication/clari-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Revenue Operations
- Forecasting
- Pipeline Management
- Sales Intelligence
- Activity Intelligence
- Deal Insights
- CRM
- Conversation Intelligence
- B2B
- Enterprise
---
