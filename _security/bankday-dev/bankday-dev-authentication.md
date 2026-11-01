---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bankday-dev-account-api-openapi.yml
  format: yaml
  label: bankday-dev Account API
  slug: bankday-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-account-api-openapi.yml
- filename: bankday-dev-ach-api-openapi.yml
  format: yaml
  label: bankday-dev Ach API
  slug: bankday-dev-ach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-ach-api-openapi.yml
- filename: bankday-dev-business-day-api-openapi.yml
  format: yaml
  label: bankday-dev Business Day API
  slug: bankday-dev-business-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-business-day-api-openapi.yml
- filename: bankday-dev-business-days-api-openapi.yml
  format: yaml
  label: bankday-dev Business Days API
  slug: bankday-dev-business-days-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-business-days-api-openapi.yml
- filename: bankday-dev-calendars-api-openapi.yml
  format: yaml
  label: bankday-dev Calendars API
  slug: bankday-dev-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-calendars-api-openapi.yml
- filename: bankday-dev-fx-api-openapi.yml
  format: yaml
  label: bankday-dev Fx API
  slug: bankday-dev-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-fx-api-openapi.yml
- filename: bankday-dev-holidays-api-openapi.yml
  format: yaml
  label: bankday-dev Holidays API
  slug: bankday-dev-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-holidays-api-openapi.yml
- filename: bankday-dev-minimum-wage-api-openapi.yml
  format: yaml
  label: bankday-dev Minimum Wage API
  slug: bankday-dev-minimum-wage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-minimum-wage-api-openapi.yml
- filename: bankday-dev-payroll-api-openapi.yml
  format: yaml
  label: bankday-dev Payroll API
  slug: bankday-dev-payroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-payroll-api-openapi.yml
- filename: bankday-dev-today-api-openapi.yml
  format: yaml
  label: bankday-dev Today API
  slug: bankday-dev-today-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-today-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bankday Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: bankday-dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: bankday-dev
provider_slug: bankday-dev
scheme_count: 1
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/bankday-dev-openapi.json
  type: http
slug: bankday-dev-authentication
source_filename: bankday-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/bankday-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bankday-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bankday-dev/authentication/bankday-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Calendar
- API
- Payments
---
