---
api_key_in: []
api_specs:
- filename: schoology-assignments-api-openapi.yml
  format: yaml
  label: Schoology Assignments API
  slug: schoology-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-assignments-api-openapi.yml
- filename: schoology-courses-api-openapi.yml
  format: yaml
  label: Schoology Courses API
  slug: schoology-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-courses-api-openapi.yml
- filename: schoology-enrollments-api-openapi.yml
  format: yaml
  label: Schoology Enrollments API
  slug: schoology-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-enrollments-api-openapi.yml
- filename: schoology-grades-api-openapi.yml
  format: yaml
  label: Schoology Grades API
  slug: schoology-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-grades-api-openapi.yml
- filename: schoology-groups-api-openapi.yml
  format: yaml
  label: Schoology Groups API
  slug: schoology-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-groups-api-openapi.yml
- filename: schoology-multi-call-api-openapi.yml
  format: yaml
  label: Schoology Multi-Call API
  slug: schoology-multi-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-multi-call-api-openapi.yml
- filename: schoology-sections-api-openapi.yml
  format: yaml
  label: Schoology Sections API
  slug: schoology-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-sections-api-openapi.yml
- filename: schoology-submissions-api-openapi.yml
  format: yaml
  label: Schoology Submissions API
  slug: schoology-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-submissions-api-openapi.yml
- filename: schoology-subscriptions-api-openapi.yml
  format: yaml
  label: Schoology Subscriptions API
  slug: schoology-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-subscriptions-api-openapi.yml
- filename: schoology-targets-api-openapi.yml
  format: yaml
  label: Schoology Targets API
  slug: schoology-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-targets-api-openapi.yml
- filename: schoology-users-api-openapi.yml
  format: yaml
  label: Schoology Users API
  slug: schoology-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-users-api-openapi.yml
- filename: schoology-events-api-openapi.yml
  format: yaml
  label: Schoology Events API
  slug: schoology-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-events-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Schoology Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Schoology secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Schoology
provider_slug: schoology
scheme_count: 1
schemes:
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  sources:
  - openapi/schoology-openapi.yml
  - openapi/schoology-webhooks-openapi.yml
  type: oauth2
slug: schoology-authentication
source_filename: schoology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/schoology-openapi.yml, openapi/schoology-webhooks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n    scopes: 0\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n  sources:\n  - openapi/schoology-openapi.yml\n  - openapi/schoology-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/authentication/schoology-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- EdTech
- LMS
- K-12
---
