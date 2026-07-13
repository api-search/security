---
api_key_in: []
api_specs:
- filename: remote-companies-api-openapi.yml
  format: yaml
  label: Remote Companies API
  slug: remote-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-companies-api-openapi.yml
- filename: remote-employments-api-openapi.yml
  format: yaml
  label: Remote Employments API
  slug: remote-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-employments-api-openapi.yml
- filename: remote-contractors-api-openapi.yml
  format: yaml
  label: Remote Contractors API
  slug: remote-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-contractors-api-openapi.yml
- filename: remote-payroll-billing-api-openapi.yml
  format: yaml
  label: Remote Payroll and Billing API
  slug: remote-payroll-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-payroll-billing-api-openapi.yml
- filename: remote-time-attendance-api-openapi.yml
  format: yaml
  label: Remote Time and Attendance API
  slug: remote-time-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-time-attendance-api-openapi.yml
- filename: remote-benefits-api-openapi.yml
  format: yaml
  label: Remote Benefits API
  slug: remote-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-benefits-api-openapi.yml
- filename: remote-files-api-openapi.yml
  format: yaml
  label: Remote Files and Custom Fields API
  slug: remote-files-and-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-files-api-openapi.yml
- filename: remote-oauth-api-openapi.yml
  format: yaml
  label: Remote OAuth 2.0 API
  slug: remote-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-oauth-api-openapi.yml
- filename: remote-webhooks-asyncapi.yml
  format: yaml
  label: Remote Webhooks
  slug: remote-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/asyncapi/remote-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Remote Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Remote secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Remote
provider_slug: remote-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/remote-benefits-api-openapi.yml
  - openapi/remote-companies-api-openapi.yml
  - openapi/remote-contractors-api-openapi.yml
  - openapi/remote-employments-api-openapi.yml
  - openapi/remote-files-api-openapi.yml
  - openapi/remote-payroll-billing-api-openapi.yml
  - openapi/remote-time-attendance-api-openapi.yml
  type: http
slug: remote-com-authentication
source_filename: remote-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/remote-benefits-api-openapi.yml, openapi/remote-companies-api-openapi.yml, openapi/remote-contractors-api-openapi.yml,\n  openapi/remote-employments-api-openapi.yml, openapi/remote-files-api-openapi.yml, openapi/remote-payroll-billing-api-openapi.yml,\n  openapi/remote-time-attendance-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/remote-benefits-api-openapi.yml\n  - openapi/remote-companies-api-openapi.yml\n  - openapi/remote-contractors-api-openapi.yml\n  - openapi/remote-employments-api-openapi.yml\n  - openapi/remote-files-api-openapi.yml\n  - openapi/remote-payroll-billing-api-openapi.yml\n  - openapi/remote-time-attendance-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/authentication/remote-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Global Payroll
- EOR
- Contractor Management
- Contractor of Record
- PEO
- HRIS
- Recruiting
- Benefits
- Employment
- HR
- Compliance
- Workforce
- MCP
- AI Agents
---
