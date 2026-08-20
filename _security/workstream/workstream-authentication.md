---
api_key_in: []
api_specs:
- filename: workstream-applicants-api-openapi.yml
  format: yaml
  label: Workstream Applicants API
  slug: workstream-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-applicants-api-openapi.yml
- filename: workstream-authorization-api-openapi.yml
  format: yaml
  label: Workstream Authorization API
  slug: workstream-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-authorization-api-openapi.yml
- filename: workstream-company-roles-api-openapi.yml
  format: yaml
  label: Workstream Company Roles API
  slug: workstream-company-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-company-roles-api-openapi.yml
- filename: workstream-company-users-api-openapi.yml
  format: yaml
  label: Workstream Company Users API
  slug: workstream-company-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-company-users-api-openapi.yml
- filename: workstream-custom-field-api-openapi.yml
  format: yaml
  label: Workstream Custom Field API
  slug: workstream-custom-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-custom-field-api-openapi.yml
- filename: workstream-departments-api-openapi.yml
  format: yaml
  label: Workstream Departments API
  slug: workstream-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-departments-api-openapi.yml
- filename: workstream-employee-documents-api-openapi.yml
  format: yaml
  label: Workstream Employee Documents API
  slug: workstream-employee-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-employee-documents-api-openapi.yml
- filename: workstream-employees-api-openapi.yml
  format: yaml
  label: Workstream Employees API
  slug: workstream-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-employees-api-openapi.yml
- filename: workstream-imported-employee-infos-api-openapi.yml
  format: yaml
  label: Workstream Imported Employee Infos API
  slug: workstream-imported-employee-infos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-imported-employee-infos-api-openapi.yml
- filename: workstream-locations-api-openapi.yml
  format: yaml
  label: Workstream Locations API
  slug: workstream-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-locations-api-openapi.yml
- filename: workstream-positions-api-openapi.yml
  format: yaml
  label: Workstream Positions API
  slug: workstream-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-positions-api-openapi.yml
- filename: workstream-team-members-api-openapi.yml
  format: yaml
  label: Workstream Team Members API
  slug: workstream-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-team-members-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workstream Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Workstream secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Workstream
provider_slug: workstream
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://public-api.workstream.us/
    flow: implicit
    scopes: 10
  name: oauth2
  sources:
  - openapi/workstream-public-api-openapi-original.json
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workstream-public-api-openapi-original.json
  type: http
slug: workstream-authentication
source_filename: workstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/workstream-public-api-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://public-api.workstream.us/\n    scopes: 10\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/authentication/workstream-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- HR Tech
- Hiring
- Payroll
- Onboarding
- Applicant Tracking
- Hourly Workforce
- Restaurant
---
