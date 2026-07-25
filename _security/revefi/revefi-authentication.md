---
api_key_in:
- header
api_specs:
- filename: revefi-create-a-custom-data-quality-monitor-api-openapi.yml
  format: yaml
  label: Revefi Create a Custom Data Quality Monitor API
  slug: revefi-create-a-custom-data-quality-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-create-a-custom-data-quality-monitor-api-openapi.yml
- filename: revefi-delete-an-existing-custom-data-quality-monitor-api-openapi.yml
  format: yaml
  label: Revefi Delete an existing Custom Data Quality Monitor API
  slug: revefi-delete-an-existing-custom-data-quality-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-delete-an-existing-custom-data-quality-monitor-api-openapi.yml
- filename: revefi-get-custom-data-quality-monitors-api-openapi.yml
  format: yaml
  label: Revefi Get Custom Data Quality Monitors API
  slug: revefi-get-custom-data-quality-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-get-custom-data-quality-monitors-api-openapi.yml
- filename: revefi-get-custom-data-quality-monitors-by-artifact-api-openapi.yml
  format: yaml
  label: Revefi Get Custom Data Quality Monitors by Artifact API
  slug: revefi-get-custom-data-quality-monitors-by-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-get-custom-data-quality-monitors-by-artifact-api-openapi.yml
- filename: revefi-run-monitors-api-openapi.yml
  format: yaml
  label: Revefi Run Monitors API
  slug: revefi-run-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-run-monitors-api-openapi.yml
- filename: revefi-update-an-existing-custom-data-quality-monitor-api-openapi.yml
  format: yaml
  label: Revefi Update an existing Custom Data Quality Monitor API
  slug: revefi-update-an-existing-custom-data-quality-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-update-an-existing-custom-data-quality-monitor-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revefi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revefi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revefi
provider_slug: revefi
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/revefi-data-quality-monitors-openapi-original.yml
  type: apiKey
slug: revefi-authentication
source_filename: revefi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/revefi-data-quality-monitors-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/revefi-data-quality-monitors-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/authentication/revefi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data
- Data Quality
- Data Observability
- FinOps
- Cost Optimization
- Analytics
- Snowflake
- Databricks
- BigQuery
- Artificial Intelligence
- MCP
---
