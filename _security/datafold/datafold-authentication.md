---
api_key_in:
- header
api_specs:
- filename: introduction
  format: yaml
  label: Datafold REST API
  slug: datafold-rest-api
  spec_type: OpenAPI
  url: https://docs.datafold.com/api-reference/introduction
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Datafold Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafold secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datafold
provider_slug: datafold
scheme_count: 1
schemes:
- description: Use the 'Authorization' header with the format 'Key <api-key>'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/datafold-openapi.json
  type: apiKey
slug: datafold-authentication
source_filename: datafold-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datafold-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Use the 'Authorization' header with the format 'Key <api-key>'\n  sources:\n  - openapi/datafold-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/authentication/datafold-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Reliability
- Data Diff
- Data Quality
- Column-Level Lineage
- Data Pipelines
- CI/CD Integration
- Anomaly Detection
- Data Observability
- Data Migrations
---
