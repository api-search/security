---
api_key_in: []
api_specs:
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Employees API
  slug: workmotion-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Contracts API
  slug: workmotion-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Onboarding API
  slug: workmotion-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Absences API
  slug: workmotion-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Documents API
  slug: workmotion-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Cost Calculator API
  slug: workmotion-cost-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Webhooks API
  slug: workmotion-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workmotion Authentication
name_suffix: Authentication
oauth_flows: []
overview: WorkMotion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WorkMotion
provider_slug: workmotion
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token supplied as a Bearer token in the Authorization header. Partner credentials are issued by WorkMotion.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workmotion-openapi.yml
  type: http
slug: workmotion-authentication
source_filename: workmotion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workmotion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token supplied as a Bearer token in the Authorization header.\n    Partner credentials are issued by WorkMotion.\n  sources:\n  - openapi/workmotion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/authentication/workmotion-authentication.yml
summary_line: http · 1 scheme
tags:
- Employer of Record
- EOR
- Global Employment
- HR
- Payroll
- Onboarding
- Contractors
- Compliance
---
