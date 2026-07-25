---
api_key_in:
- header
api_specs:
- filename: sage-hr-documents-api-openapi.yml
  format: yaml
  label: Sage HR Documents API
  slug: sage-hr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-documents-api-openapi.yml
- filename: sage-hr-employee-api-openapi.yml
  format: yaml
  label: Sage HR Employee API
  slug: sage-hr-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-employee-api-openapi.yml
- filename: sage-hr-integrations-api-openapi.yml
  format: yaml
  label: Sage HR Integrations API
  slug: sage-hr-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-integrations-api-openapi.yml
- filename: sage-hr-kit-days-api-openapi.yml
  format: yaml
  label: Sage HR KIT days API
  slug: sage-hr-kit-days-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-kit-days-api-openapi.yml
- filename: sage-hr-leave-management-api-openapi.yml
  format: yaml
  label: Sage HR Leave management API
  slug: sage-hr-leave-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-leave-management-api-openapi.yml
- filename: sage-hr-offboarding-api-openapi.yml
  format: yaml
  label: Sage HR Offboarding API
  slug: sage-hr-offboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-offboarding-api-openapi.yml
- filename: sage-hr-onboarding-api-openapi.yml
  format: yaml
  label: Sage HR Onboarding API
  slug: sage-hr-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-onboarding-api-openapi.yml
- filename: sage-hr-performance-api-openapi.yml
  format: yaml
  label: Sage HR Performance API
  slug: sage-hr-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-performance-api-openapi.yml
- filename: sage-hr-policies-api-openapi.yml
  format: yaml
  label: Sage HR Policies API
  slug: sage-hr-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-policies-api-openapi.yml
- filename: sage-hr-positions-api-openapi.yml
  format: yaml
  label: Sage HR Positions API
  slug: sage-hr-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-positions-api-openapi.yml
- filename: sage-hr-recruitment-api-openapi.yml
  format: yaml
  label: Sage HR Recruitment API
  slug: sage-hr-recruitment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-recruitment-api-openapi.yml
- filename: sage-hr-teams-api-openapi.yml
  format: yaml
  label: Sage HR Teams API
  slug: sage-hr-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-teams-api-openapi.yml
- filename: sage-hr-terminations-reasons-api-openapi.yml
  format: yaml
  label: Sage HR Terminations reasons API
  slug: sage-hr-terminations-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-terminations-reasons-api-openapi.yml
- filename: sage-hr-timesheets-api-openapi.yml
  format: yaml
  label: Sage HR Timesheets API
  slug: sage-hr-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-timesheets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sage Hr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sage HR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sage HR
provider_slug: sage-hr
scheme_count: 1
schemes:
- description: All request are required to pass a `X-Auth-Token` header.
  in: header
  name: api_key
  parameter: X-Auth-Token
  sources:
  - openapi/sage-hr-openapi.yml
  type: apiKey
slug: sage-hr-authentication
source_filename: sage-hr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sage-hr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: All request are required to pass a `X-Auth-Token` header.\n  sources:\n  - openapi/sage-hr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/authentication/sage-hr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- HR
- HRIS
- People
- SMB
- Leave Management
- Recruitment
- Performance
- Timesheets
- Onboarding
---
