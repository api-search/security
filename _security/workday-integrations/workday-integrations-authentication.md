---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Workday REST API
  slug: workday-rest-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/restapi/openapi.json
- filename: workday-integrations-raas-openapi.yml
  format: yaml
  label: Workday RaaS (Report-as-a-Service)
  slug: workday-raas-report-as-a-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-raas-openapi.yml
- filename: workday-integrations-prism-analytics-openapi.yml
  format: yaml
  label: Workday Prism Analytics API
  slug: workday-prism-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-prism-analytics-openapi.yml
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
