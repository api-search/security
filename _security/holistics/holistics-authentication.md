---
api_key_in:
- header
api_specs:
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Data Schedules & Jobs API
  slug: holistics-data-schedules-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Dashboards & Reports API
  slug: holistics-dashboards-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Export API
  slug: holistics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Users & Permissions API
  slug: holistics-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Embedded Analytics API
  slug: holistics-embedded-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Holistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Holistics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Holistics
provider_slug: holistics
scheme_count: 1
schemes:
- description: Per-user API key generated from Holistics user settings.
  in: header
  name: HolisticsKey
  parameter: X-Holistics-Key
  sources:
  - openapi/holistics-openapi.yml
  type: apiKey
slug: holistics-authentication
source_filename: holistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/holistics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HolisticsKey\n  type: apiKey\n  in: header\n  parameter: X-Holistics-Key\n  description: Per-user API key generated from Holistics user settings.\n  sources:\n  - openapi/holistics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/authentication/holistics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Intelligence
- Analytics
- Self-Service BI
- Data Modeling
- Embedded Analytics
---
