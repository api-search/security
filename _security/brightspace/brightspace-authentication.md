---
api_key_in: []
api_specs:
- filename: brightspace-assignments-api-openapi.yml
  format: yaml
  label: D2L Brightspace Assignments API
  slug: brightspace-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-assignments-api-openapi.yml
- filename: brightspace-calendar-api-openapi.yml
  format: yaml
  label: D2L Brightspace Calendar API
  slug: brightspace-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-calendar-api-openapi.yml
- filename: brightspace-content-api-openapi.yml
  format: yaml
  label: D2L Brightspace Content API
  slug: brightspace-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-content-api-openapi.yml
- filename: brightspace-data-hub-api-openapi.yml
  format: yaml
  label: D2L Brightspace Data Hub API
  slug: brightspace-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-data-hub-api-openapi.yml
- filename: brightspace-discussions-api-openapi.yml
  format: yaml
  label: D2L Brightspace Discussions API
  slug: brightspace-discussions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-discussions-api-openapi.yml
- filename: brightspace-enrollments-api-openapi.yml
  format: yaml
  label: D2L Brightspace Enrollments API
  slug: brightspace-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-enrollments-api-openapi.yml
- filename: brightspace-grades-api-openapi.yml
  format: yaml
  label: D2L Brightspace Grades API
  slug: brightspace-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-grades-api-openapi.yml
- filename: brightspace-learning-outcomes-api-openapi.yml
  format: yaml
  label: D2L Brightspace Learning Outcomes API
  slug: brightspace-learning-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-learning-outcomes-api-openapi.yml
- filename: brightspace-news-api-openapi.yml
  format: yaml
  label: D2L Brightspace News API
  slug: brightspace-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-news-api-openapi.yml
- filename: brightspace-org-units-api-openapi.yml
  format: yaml
  label: D2L Brightspace Org Units API
  slug: brightspace-org-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-org-units-api-openapi.yml
- filename: brightspace-quizzes-api-openapi.yml
  format: yaml
  label: D2L Brightspace Quizzes API
  slug: brightspace-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-quizzes-api-openapi.yml
- filename: brightspace-users-api-openapi.yml
  format: yaml
  label: D2L Brightspace Users API
  slug: brightspace-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-users-api-openapi.yml
- filename: brightspace-versions-api-openapi.yml
  format: yaml
  label: D2L Brightspace Versions API
  slug: brightspace-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-versions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Brightspace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: D2L Brightspace secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: D2L Brightspace
provider_slug: brightspace
scheme_count: 1
schemes:
- description: OAuth 2 authorization code grant. Tokens are issued by the D2L auth service. Scopes take the form group:resource:action (for example users:userdata:read).
  flows:
  - authorizationUrl: https://auth.brightspace.com/oauth2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.brightspace.com/core/connect/token
  name: oauth2
  sources:
  - openapi/brightspace-openapi.yml
  type: oauth2
slug: brightspace-authentication
source_filename: brightspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brightspace-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.brightspace.com/oauth2/auth\n    tokenUrl: https://auth.brightspace.com/core/connect/token\n    scopes: 4\n  description: OAuth 2 authorization code grant. Tokens are issued by the D2L auth service.\n    Scopes take the form group:resource:action (for example users:userdata:read).\n  sources:\n  - openapi/brightspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/authentication/brightspace-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- LMS
- Learning Management System
- EdTech
- Education
- Valence
- D2L
- Brightspace
---
