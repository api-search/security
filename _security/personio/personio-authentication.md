---
api_key_in: []
api_specs:
- filename: personio-absence-periods-api-openapi.yml
  format: yaml
  label: Personio Absence Periods API
  slug: personio-absence-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/openapi/personio-absence-periods-api-openapi.yml
- filename: personio-auth-api-openapi.yml
  format: yaml
  label: Personio Auth API
  slug: personio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/openapi/personio-auth-api-openapi.yml
- filename: personio-persons-api-openapi.yml
  format: yaml
  label: Personio Persons API
  slug: personio-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/openapi/personio-persons-api-openapi.yml
- filename: personio-projects-api-openapi.yml
  format: yaml
  label: Personio Projects API
  slug: personio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/openapi/personio-projects-api-openapi.yml
- filename: personio-webhooks-api-openapi.yml
  format: yaml
  label: Personio Webhooks API
  slug: personio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/openapi/personio-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Personio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Personio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Personio
provider_slug: personio
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer access token obtained from POST /v2/auth/token using the

    OAuth 2.0 Client Credentials grant.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/personio-openapi.yml
  type: http
slug: personio-authentication
source_filename: personio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/personio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Bearer access token obtained from POST /v2/auth/token using the\n    OAuth 2.0 Client Credentials grant.\n  sources:\n  - openapi/personio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/authentication/personio-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- HRIS
- Recruiting
- Applicant Tracking
- Absence Management
- Time Tracking
- Europe HR
---
