---
api_key_in:
- header
api_specs:
- filename: toro-crews-api-openapi.yml
  format: yaml
  label: Toro Crews API
  slug: toro-crews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-crews-api-openapi.yml
- filename: toro-customers-api-openapi.yml
  format: yaml
  label: Toro Customers API
  slug: toro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-customers-api-openapi.yml
- filename: toro-equipment-api-openapi.yml
  format: yaml
  label: Toro Equipment API
  slug: toro-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-equipment-api-openapi.yml
- filename: toro-invoices-api-openapi.yml
  format: yaml
  label: Toro Invoices API
  slug: toro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-invoices-api-openapi.yml
- filename: toro-irrigation-api-openapi.yml
  format: yaml
  label: Toro Irrigation API
  slug: toro-irrigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-irrigation-api-openapi.yml
- filename: toro-jobs-api-openapi.yml
  format: yaml
  label: Toro Jobs API
  slug: toro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-jobs-api-openapi.yml
- filename: toro-payments-api-openapi.yml
  format: yaml
  label: Toro Payments API
  slug: toro-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-payments-api-openapi.yml
- filename: toro-reports-api-openapi.yml
  format: yaml
  label: Toro Reports API
  slug: toro-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-reports-api-openapi.yml
- filename: toro-schedules-api-openapi.yml
  format: yaml
  label: Toro Schedules API
  slug: toro-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-schedules-api-openapi.yml
- filename: toro-sensors-api-openapi.yml
  format: yaml
  label: Toro Sensors API
  slug: toro-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-sensors-api-openapi.yml
- filename: toro-zones-api-openapi.yml
  format: yaml
  label: Toro Zones API
  slug: toro-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-zones-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toro secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Toro
provider_slug: toro
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/toro-horizon360-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/toro-intellidash-openapi.yml
  type: apiKey
slug: toro-authentication
source_filename: toro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toro-horizon360-openapi.yml, openapi/toro-intellidash-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/toro-horizon360-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/toro-intellidash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/authentication/toro-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Landscaping
- Irrigation
- Golf
- Equipment
- Smart Connected Products
- Fleet Management
- Turf Management
- Fortune 1000
---
