---
api_key_in:
- header
api_specs:
- filename: acceldata-adoc-api.yaml
  format: yaml
  label: Acceldata Data Observability Cloud API
  slug: adoc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-adoc-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Acceldata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acceldata secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Acceldata
provider_slug: acceldata
scheme_count: 1
schemes:
- description: Acceldata API key for authentication
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/acceldata-adoc-api.yaml
  type: apiKey
slug: acceldata-authentication
source_filename: acceldata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acceldata-adoc-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Acceldata API key for authentication\n  sources:\n  - openapi/acceldata-adoc-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/authentication/acceldata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
---
