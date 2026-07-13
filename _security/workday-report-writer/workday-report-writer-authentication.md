---
api_key_in: []
api_specs:
- filename: workday-report-writer-raas-openapi.yml
  format: yaml
  label: Workday Report-as-a-Service (RaaS) REST API
  slug: workday-report-as-a-service-raas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-raas-openapi.yml
- filename: workday-report-writer-wql-openapi.yml
  format: yaml
  label: Workday WQL API
  slug: workday-wql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-wql-openapi.yml
- filename: workday-report-writer-prism-analytics-openapi.yml
  format: yaml
  label: Workday Prism Analytics API
  slug: workday-prism-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-prism-analytics-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workday Report Writer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workday Report Writer secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Workday Report Writer
provider_slug: workday-report-writer
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from Workday token endpoint. Requires the Prism Analytics scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workday-report-writer-prism-analytics-openapi.yml
  - openapi/workday-report-writer-raas-openapi.yml
  - openapi/workday-report-writer-wql-openapi.yml
  type: http
- description: HTTP Basic authentication using an Integration System User (ISU) username and password configured in Workday
  name: basicAuth
  scheme: basic
  sources:
  - openapi/workday-report-writer-raas-openapi.yml
  type: http
slug: workday-report-writer-authentication
source_filename: workday-report-writer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-report-writer-prism-analytics-openapi.yml, openapi/workday-report-writer-raas-openapi.yml,\n  openapi/workday-report-writer-wql-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from Workday token endpoint. Requires the Prism\n    Analytics scope.\n  sources:\n  - openapi/workday-report-writer-prism-analytics-openapi.yml\n  - openapi/workday-report-writer-raas-openapi.yml\n  - openapi/workday-report-writer-wql-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using an Integration System User (ISU) username and\n    password configured in Workday\n  sources:\n  - openapi/workday-report-writer-raas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/authentication/workday-report-writer-authentication.yml
summary_line: http · 2 schemes
tags:
- Analytics
- Enterprise
- Erp
- Financials
- Hrms
- Reporting
- Saas
---
