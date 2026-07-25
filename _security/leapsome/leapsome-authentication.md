---
api_key_in: []
api_specs:
- filename: leapsome-absences-api-openapi.yml
  format: yaml
  label: Leapsome absences API
  slug: leapsome-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-absences-api-openapi.yml
- filename: leapsome-accessroles-api-openapi.yml
  format: yaml
  label: Leapsome accessRoles API
  slug: leapsome-accessroles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-accessroles-api-openapi.yml
- filename: leapsome-auth-api-openapi.yml
  format: yaml
  label: Leapsome auth API
  slug: leapsome-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-auth-api-openapi.yml
- filename: leapsome-documents-api-openapi.yml
  format: yaml
  label: Leapsome documents API
  slug: leapsome-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-documents-api-openapi.yml
- filename: leapsome-feedback-api-openapi.yml
  format: yaml
  label: Leapsome feedback API
  slug: leapsome-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-feedback-api-openapi.yml
- filename: leapsome-goals-api-openapi.yml
  format: yaml
  label: Leapsome goals API
  slug: leapsome-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-goals-api-openapi.yml
- filename: leapsome-groups-api-openapi.yml
  format: yaml
  label: Leapsome Groups API
  slug: leapsome-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-groups-api-openapi.yml
- filename: leapsome-leapsome-api-api-openapi.yml
  format: yaml
  label: Leapsome Leapsome API API
  slug: leapsome-leapsome-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-leapsome-api-api-openapi.yml
- filename: leapsome-payroll-api-openapi.yml
  format: yaml
  label: Leapsome payroll API
  slug: leapsome-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-payroll-api-openapi.yml
- filename: leapsome-reviews-api-openapi.yml
  format: yaml
  label: Leapsome reviews API
  slug: leapsome-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-reviews-api-openapi.yml
- filename: leapsome-schemas-api-openapi.yml
  format: yaml
  label: Leapsome Schemas API
  slug: leapsome-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-schemas-api-openapi.yml
- filename: leapsome-timetracking-api-openapi.yml
  format: yaml
  label: Leapsome timeTracking API
  slug: leapsome-timetracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-timetracking-api-openapi.yml
- filename: leapsome-users-api-openapi.yml
  format: yaml
  label: Leapsome users API
  slug: leapsome-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-users-api-openapi.yml
- filename: leapsome-worklocations-api-openapi.yml
  format: yaml
  label: Leapsome workLocations API
  slug: leapsome-worklocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-worklocations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leapsome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leapsome secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leapsome
provider_slug: leapsome
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/leapsome-content-api-openapi.yml
  - openapi/leapsome-scim-api-openapi.yml
  type: http
slug: leapsome-authentication
source_filename: leapsome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leapsome-content-api-openapi.yml, openapi/leapsome-scim-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/leapsome-content-api-openapi.yml\n  - openapi/leapsome-scim-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/authentication/leapsome-authentication.yml
summary_line: http · 1 scheme
tags:
- People Enablement
- Performance Management
- OKRs
- Goals
- Engagement Surveys
- HRIS
- SCIM
- Employee Development
- 1:1 Meetings
- Learning
---
