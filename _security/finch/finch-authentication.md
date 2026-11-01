---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finch-connect-api-openapi.yml
  format: yaml
  label: Finch Connect API
  slug: finch-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-connect-api-openapi.yml
- filename: finch-benefits-api-openapi.yml
  format: yaml
  label: Finch Benefits API
  slug: finch-benefits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-benefits-api-openapi.yml
- filename: finch-deductions-api-openapi.yml
  format: yaml
  label: Finch Deductions API
  slug: finch-deductions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-deductions-api-openapi.yml
- filename: finch-documents-api-openapi.yml
  format: yaml
  label: Finch Documents API
  slug: finch-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-documents-api-openapi.yml
- filename: finch-management-api-openapi.yml
  format: yaml
  label: Finch Management API
  slug: finch-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-management-api-openapi.yml
- filename: finch-organization-api-openapi.yml
  format: yaml
  label: Finch Organization API
  slug: finch-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-organization-api-openapi.yml
- filename: finch-payroll-api-openapi.yml
  format: yaml
  label: Finch Payroll API
  slug: finch-payroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-payroll-api-openapi.yml
- filename: finch-sandbox-api-openapi.yml
  format: yaml
  label: Finch Sandbox API
  slug: finch-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finch/openapi/finch-sandbox-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Finch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finch
provider_slug: finch
scheme_count: 1
schemes:
- bearerFormat: Finch access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/finch-openapi.yml
  type: http
slug: finch-authentication
source_filename: finch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/finch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Finch access token\n  sources:\n  - openapi/finch-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/finch/authentication/finch-authentication.yml
summary_line: http · 1 scheme
tags:
- Employment
- HRIS
- Payroll
- Benefits
- Human Resources
- Unified API
- Workforce
- Integration
- Employee Benefits
---
