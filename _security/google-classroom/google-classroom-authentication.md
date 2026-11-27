---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-classroom-courses-api-openapi.yml
  format: yaml
  label: Google Classroom Courses API
  slug: google-classroom-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-courses-api-openapi.yml
- filename: google-classroom-invitations-api-openapi.yml
  format: yaml
  label: Google Classroom Invitations API
  slug: google-classroom-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-invitations-api-openapi.yml
- filename: google-classroom-registrations-api-openapi.yml
  format: yaml
  label: Google Classroom Registrations API
  slug: google-classroom-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-registrations-api-openapi.yml
- filename: google-classroom-user-profiles-api-openapi.yml
  format: yaml
  label: Google Classroom User Profiles API
  slug: google-classroom-user-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-user-profiles-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Classroom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Classroom secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Classroom
provider_slug: google-classroom
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-classroom-registrations-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 24
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-classroom-registrations-api-openapi.yml
  type: oauth2
slug: google-classroom-authentication
source_filename: google-classroom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-classroom-registrations-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 24\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-classroom/authentication/google-classroom-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Assignments
- Classroom
- Courses
- Education
- Google
- Google Workspace
- Students
---
