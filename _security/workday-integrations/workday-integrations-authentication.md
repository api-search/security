---
api_key_in: []
api_specs:
- filename: workday-integrations-benefits-api-openapi.yml
  format: yaml
  label: Workday Integrations Benefits API
  slug: workday-integrations-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-benefits-api-openapi.yml
- filename: workday-integrations-business-processes-api-openapi.yml
  format: yaml
  label: Workday Integrations Business Processes API
  slug: workday-integrations-business-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-business-processes-api-openapi.yml
- filename: workday-integrations-compensation-api-openapi.yml
  format: yaml
  label: Workday Integrations Compensation API
  slug: workday-integrations-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-compensation-api-openapi.yml
- filename: workday-integrations-data-sources-api-openapi.yml
  format: yaml
  label: Workday Integrations Data Sources API
  slug: workday-integrations-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-data-sources-api-openapi.yml
- filename: workday-integrations-data-upload-api-openapi.yml
  format: yaml
  label: Workday Integrations Data Upload API
  slug: workday-integrations-data-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-data-upload-api-openapi.yml
- filename: workday-integrations-datasets-api-openapi.yml
  format: yaml
  label: Workday Integrations Datasets API
  slug: workday-integrations-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-datasets-api-openapi.yml
- filename: workday-integrations-job-profiles-api-openapi.yml
  format: yaml
  label: Workday Integrations Job Profiles API
  slug: workday-integrations-job-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-job-profiles-api-openapi.yml
- filename: workday-integrations-organizations-api-openapi.yml
  format: yaml
  label: Workday Integrations Organizations API
  slug: workday-integrations-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-organizations-api-openapi.yml
- filename: workday-integrations-payroll-api-openapi.yml
  format: yaml
  label: Workday Integrations Payroll API
  slug: workday-integrations-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-payroll-api-openapi.yml
- filename: workday-integrations-positions-api-openapi.yml
  format: yaml
  label: Workday Integrations Positions API
  slug: workday-integrations-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-positions-api-openapi.yml
- filename: workday-integrations-recruiting-api-openapi.yml
  format: yaml
  label: Workday Integrations Recruiting API
  slug: workday-integrations-recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-recruiting-api-openapi.yml
- filename: workday-integrations-report-metadata-api-openapi.yml
  format: yaml
  label: Workday Integrations Report Metadata API
  slug: workday-integrations-report-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-report-metadata-api-openapi.yml
- filename: workday-integrations-reports-api-openapi.yml
  format: yaml
  label: Workday Integrations Reports API
  slug: workday-integrations-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-reports-api-openapi.yml
- filename: workday-integrations-tables-api-openapi.yml
  format: yaml
  label: Workday Integrations Tables API
  slug: workday-integrations-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-tables-api-openapi.yml
- filename: workday-integrations-time-off-api-openapi.yml
  format: yaml
  label: Workday Integrations Time Off API
  slug: workday-integrations-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-time-off-api-openapi.yml
- filename: workday-integrations-workers-api-openapi.yml
  format: yaml
  label: Workday Integrations Workers API
  slug: workday-integrations-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-workers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workday Integrations Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workday Integrations secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Workday Integrations
provider_slug: workday-integrations
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained via Workday authentication for Prism Analytics API access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workday-integrations-prism-analytics-openapi.yml
  - openapi/workday-integrations-raas-openapi.yml
  - openapi/workday-integrations-rest-api-openapi.yml
  type: http
- description: HTTP Basic authentication using Workday integration system user credentials (ISU username and password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/workday-integrations-raas-openapi.yml
  type: http
slug: workday-integrations-authentication
source_filename: workday-integrations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-integrations-prism-analytics-openapi.yml, openapi/workday-integrations-raas-openapi.yml,\n  openapi/workday-integrations-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained via Workday authentication for Prism Analytics\n    API access.\n  sources:\n  - openapi/workday-integrations-prism-analytics-openapi.yml\n  - openapi/workday-integrations-raas-openapi.yml\n  - openapi/workday-integrations-rest-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using Workday integration system user credentials (ISU\n    username and password).\n  sources:\n  - openapi/workday-integrations-raas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/authentication/workday-integrations-authentication.yml
summary_line: http · 2 schemes
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
---
