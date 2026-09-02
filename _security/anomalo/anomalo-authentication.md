---
api_key_in:
- header
api_specs:
- filename: anomalo-access-groups-api-openapi.yml
  format: yaml
  label: Anomalo Access Groups API
  slug: anomalo-access-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-access-groups-api-openapi.yml
- filename: anomalo-api-keys-api-openapi.yml
  format: yaml
  label: Anomalo API Keys API
  slug: anomalo-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-api-keys-api-openapi.yml
- filename: anomalo-check-runs-api-openapi.yml
  format: yaml
  label: Anomalo Check Runs API
  slug: anomalo-check-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-check-runs-api-openapi.yml
- filename: anomalo-checks-api-openapi.yml
  format: yaml
  label: Anomalo Checks API
  slug: anomalo-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-checks-api-openapi.yml
- filename: anomalo-document-collections-api-openapi.yml
  format: yaml
  label: Anomalo Document Collections API
  slug: anomalo-document-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-document-collections-api-openapi.yml
- filename: anomalo-documents-api-openapi.yml
  format: yaml
  label: Anomalo Documents API
  slug: anomalo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-documents-api-openapi.yml
- filename: anomalo-exports-api-openapi.yml
  format: yaml
  label: Anomalo Exports API
  slug: anomalo-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-exports-api-openapi.yml
- filename: anomalo-issues-api-openapi.yml
  format: yaml
  label: Anomalo Issues API
  slug: anomalo-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-issues-api-openapi.yml
- filename: anomalo-labels-api-openapi.yml
  format: yaml
  label: Anomalo Labels API
  slug: anomalo-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-labels-api-openapi.yml
- filename: anomalo-lineage-api-openapi.yml
  format: yaml
  label: Anomalo Lineage API
  slug: anomalo-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-lineage-api-openapi.yml
- filename: anomalo-notification-channels-api-openapi.yml
  format: yaml
  label: Anomalo Notification Channels API
  slug: anomalo-notification-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-notification-channels-api-openapi.yml
- filename: anomalo-organizations-api-openapi.yml
  format: yaml
  label: Anomalo Organizations API
  slug: anomalo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-organizations-api-openapi.yml
- filename: anomalo-sensitive-columns-api-openapi.yml
  format: yaml
  label: Anomalo Sensitive Columns API
  slug: anomalo-sensitive-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-sensitive-columns-api-openapi.yml
- filename: anomalo-system-api-openapi.yml
  format: yaml
  label: Anomalo System API
  slug: anomalo-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-system-api-openapi.yml
- filename: anomalo-tables-api-openapi.yml
  format: yaml
  label: Anomalo Tables API
  slug: anomalo-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-tables-api-openapi.yml
- filename: anomalo-tasks-api-openapi.yml
  format: yaml
  label: Anomalo Tasks API
  slug: anomalo-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-tasks-api-openapi.yml
- filename: anomalo-users-api-openapi.yml
  format: yaml
  label: Anomalo Users API
  slug: anomalo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-users-api-openapi.yml
- filename: anomalo-warehouses-api-openapi.yml
  format: yaml
  label: Anomalo Warehouses API
  slug: anomalo-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-warehouses-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anomalo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anomalo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Anomalo
provider_slug: anomalo
scheme_count: 2
schemes:
- description: Anomalo API secret token. The first-party client sends it as `X-Anomalo-Token` by default (`legacy_auth=True`), read from the `ANOMALO_API_SECRET_TOKEN` environment variable.
  in: header
  name: AnomaloToken
  parameter: X-Anomalo-Token
  sources:
  - openapi/anomalo-public-api-openapi.yml
  type: apiKey
- description: 'Anomalo API secret token sent as `Authorization: Bearer <token>`. Selected in the first-party client with `legacy_auth=False`.'
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/anomalo-public-api-openapi.yml
  type: http
slug: anomalo-authentication
source_filename: anomalo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/anomalo-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AnomaloToken\n  type: apiKey\n  in: header\n  parameter: X-Anomalo-Token\n  description: Anomalo API secret token. The first-party client sends it as `X-Anomalo-Token`\n    by default (`legacy_auth=True`), read from the `ANOMALO_API_SECRET_TOKEN` environment variable.\n  sources:\n  - openapi/anomalo-public-api-openapi.yml\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: 'Anomalo API secret token sent as `Authorization: Bearer <token>`. Selected in\n    the first-party client with `legacy_auth=False`.'\n  sources:\n  - openapi/anomalo-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/authentication/anomalo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Quality
- Data Observability
- Data Monitoring
- Anomaly Detection
- Data Governance
- Data Lineage
- Data Profiling
- Data Validation
- Data Engineering
- Machine-Learning
- Snowflake
- Databricks
- BigQuery
- Enterprise Data
- MCP
- agent-native
---
