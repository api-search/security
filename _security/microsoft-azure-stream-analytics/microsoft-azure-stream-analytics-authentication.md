---
api_key_in: []
api_specs:
- filename: microsoft-azure-stream-analytics-openapi.yml
  format: yaml
  label: Azure Stream Analytics REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-stream-analytics/refs/heads/main/openapi/microsoft-azure-stream-analytics-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Stream Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Stream Analytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure Stream Analytics
provider_slug: microsoft-azure-stream-analytics
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-azure-stream-analytics-openapi.yml
  type: http
slug: microsoft-azure-stream-analytics-authentication
source_filename: microsoft-azure-stream-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-stream-analytics-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-azure-stream-analytics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-stream-analytics/refs/heads/main/authentication/microsoft-azure-stream-analytics-authentication.yml
summary_line: http · 1 scheme
tags:
- Stream Processing
- Real-Time Analytics
- IoT
- Event Processing
---
