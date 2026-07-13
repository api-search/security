---
api_key_in: []
api_specs:
- filename: canvas.openapi.yaml
  format: yaml
  label: Canvas LMS REST API
  slug: canvas-lms-rest-api
  spec_type: OpenAPI
  url: https://github.com/instructure/canvas-lms/blob/master/public/doc/openapi/canvas.openapi.yaml
- filename: instructure-canvas-lti-openapi.yml
  format: yaml
  label: Canvas LTI 1.3 API
  slug: canvas-lti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-canvas-lti-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Instructure Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instructure secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instructure
provider_slug: instructure
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://{canvas_domain}/login/oauth2/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{canvas_domain}/login/oauth2/token
  name: oauth2
  sources:
  - openapi/instructure-canvas-lti-openapi.yml
  type: oauth2
- description: Bearer token (access token)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/instructure-canvas-lti-openapi.yml
  type: http
slug: instructure-authentication
source_filename: instructure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instructure-canvas-lti-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{canvas_domain}/login/oauth2/auth\n    tokenUrl: https://{canvas_domain}/login/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/instructure-canvas-lti-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token (access token)\n  sources:\n  - openapi/instructure-canvas-lti-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/authentication/instructure-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- EdTech
- Education
- LMS
- Canvas
- Courses
- Enrollments
- Assignments
- Grades
- Discussions
- GraphQL
- LTI
- Learning Management
---
