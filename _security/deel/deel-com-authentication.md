---
api_key_in: []
api_specs:
- filename: deel-core-api-openapi.yml
  format: yaml
  label: Deel Core API
  slug: deel-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-core-api-openapi.yml
- filename: deel-eor-api-openapi.yml
  format: yaml
  label: Deel Employer of Record (EOR) API
  slug: deel-eor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-eor-api-openapi.yml
- filename: deel-contractors-api-openapi.yml
  format: yaml
  label: Deel Contractors API
  slug: deel-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-contractors-api-openapi.yml
- filename: deel-global-payroll-api-openapi.yml
  format: yaml
  label: Deel Global Payroll API
  slug: deel-global-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-global-payroll-api-openapi.yml
- filename: deel-hris-api-openapi.yml
  format: yaml
  label: Deel HRIS API
  slug: deel-hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-hris-api-openapi.yml
- filename: deel-ats-api-openapi.yml
  format: yaml
  label: Deel ATS API
  slug: deel-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-ats-api-openapi.yml
- filename: deel-webhooks-api-openapi.yml
  format: yaml
  label: Deel Webhooks API
  slug: deel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-webhooks-api-openapi.yml
- filename: deel-platform-extensions-api-openapi.yml
  format: yaml
  label: Deel Platform Extensions API
  slug: deel-platform-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-extensions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deel Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deel
provider_slug: deel
scheme_count: 1
schemes:
- bearerFormat: opaque
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/deel-ats-api-openapi.yml
  - openapi/deel-contractors-api-openapi.yml
  - openapi/deel-core-api-openapi.yml
  - openapi/deel-eor-api-openapi.yml
  - openapi/deel-global-payroll-api-openapi.yml
  - openapi/deel-hris-api-openapi.yml
  - openapi/deel-platform-extensions-api-openapi.yml
  - openapi/deel-webhooks-api-openapi.yml
  type: http
slug: deel-com-authentication
source_filename: deel-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deel-ats-api-openapi.yml, openapi/deel-contractors-api-openapi.yml, openapi/deel-core-api-openapi.yml,\n  openapi/deel-eor-api-openapi.yml, openapi/deel-global-payroll-api-openapi.yml, openapi/deel-hris-api-openapi.yml,\n  openapi/deel-platform-extensions-api-openapi.yml, openapi/deel-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  sources:\n  - openapi/deel-ats-api-openapi.yml\n  - openapi/deel-contractors-api-openapi.yml\n  - openapi/deel-core-api-openapi.yml\n  - openapi/deel-eor-api-openapi.yml\n  - openapi/deel-global-payroll-api-openapi.yml\n  - openapi/deel-hris-api-openapi.yml\n  - openapi/deel-platform-extensions-api-openapi.yml\n  - openapi/deel-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/authentication/deel-com-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- Payroll
- Global Payroll
- EOR
- Employer of Record
- Contractors
- HRIS
- ATS
- Workforce
- Compliance
- Immigration
- Background Checks
- Webhooks
- IT
---
