---
api_key_in: []
api_specs:
- filename: Reporting.yaml
  format: yaml
  label: Workday Report as a Service (RaaS)
  slug: workday-report-as-a-service-raas
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Reporting/v1/Reporting.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workday Reporting Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workday Reporting secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Workday Reporting
provider_slug: workday-reporting
scheme_count: 2
schemes:
- description: HTTP Basic authentication using Workday integration system user credentials (ISU username and password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/workday-reporting-raas-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained via Workday authentication for report access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workday-reporting-raas-openapi.yml
  type: http
slug: workday-reporting-authentication
source_filename: workday-reporting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-reporting-raas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using Workday integration system user credentials (ISU\n    username and password).\n  sources:\n  - openapi/workday-reporting-raas-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained via Workday authentication for report access.\n  sources:\n  - openapi/workday-reporting-raas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-reporting/refs/heads/main/authentication/workday-reporting-authentication.yml
summary_line: http · 2 schemes
tags:
- Analytics
- Business Intelligence
- Financial Reporting
- Hr Data
- Reporting
---
