---
api_key_in: []
api_specs:
- filename: sesame-hr-absences-and-leave-api-openapi.yml
  format: yaml
  label: Sesame HR Absences and Leave API
  slug: sesame-hr-absences-and-leave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-absences-and-leave-api-openapi.yml
- filename: sesame-hr-departments-and-org-api-openapi.yml
  format: yaml
  label: Sesame HR Departments and Org API
  slug: sesame-hr-departments-and-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-departments-and-org-api-openapi.yml
- filename: sesame-hr-employees-api-openapi.yml
  format: yaml
  label: Sesame HR Employees API
  slug: sesame-hr-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-employees-api-openapi.yml
- filename: sesame-hr-meta-api-openapi.yml
  format: yaml
  label: Sesame HR Meta API
  slug: sesame-hr-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-meta-api-openapi.yml
- filename: sesame-hr-scheduling-api-openapi.yml
  format: yaml
  label: Sesame HR Scheduling API
  slug: sesame-hr-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-scheduling-api-openapi.yml
- filename: sesame-hr-time-tracking-api-openapi.yml
  format: yaml
  label: Sesame HR Time Tracking API
  slug: sesame-hr-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-time-tracking-api-openapi.yml
- filename: sesame-hr-webhooks-api-openapi.yml
  format: yaml
  label: Sesame HR Webhooks API
  slug: sesame-hr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/openapi/sesame-hr-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sesame Hr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sesame HR secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sesame HR
provider_slug: sesame-hr
scheme_count: 1
schemes:
- description: 'Bearer API token. Generated self-serve in the Sesame admin panel by logging in to app.sesametime.com and going to Settings > Integrations > API, then "Create New Token". Passed as `Authorization: Bearer [example key]`. Tokens grant access scoped to the account holder''s permissions, can be revoked from the dashboard (revoked tokens return 401), and are recommended to be rotated every ~90 days. Token validity can be checked with GET /core/v3/info.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://apidocs.sesametime.com/authentication
  - https://apidocs.sesametime.com/introduction
  type: http
slug: sesame-hr-authentication
source_filename: sesame-hr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: https://apidocs.sesametime.com/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer API token. Generated self-serve in the Sesame admin panel by logging\n    in to app.sesametime.com and going to Settings > Integrations > API, then\n    \"Create New Token\". Passed as `Authorization: Bearer [example key]`.\n    Tokens grant access scoped to the account holder's permissions, can be\n    revoked from the dashboard (revoked tokens return 401), and are recommended\n    to be rotated every ~90 days. Token validity can be checked with\n    GET /core/v3/info.\n  sources:\n  - https://apidocs.sesametime.com/authentication\n  - https://apidocs.sesametime.com/introduction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sesame-hr/refs/heads/main/authentication/sesame-hr-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- HRIS
- Time Tracking
- Workforce Management
- Employee Management
- HR
- Attendance
- Absence Management
- Scheduling
- Payroll
---
