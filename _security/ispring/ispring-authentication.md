---
api_key_in: []
api_specs:
- filename: rest-api
  format: yaml
  label: iSpring Learn REST API
  slug: ispring-learn-rest-api
  spec_type: OpenAPI
  url: https://api-learn.ispringlearn.com/docs/rest-api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ispring Authentication
name_suffix: Authentication
oauth_flows: []
overview: iSpring Learn secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iSpring Learn
provider_slug: ispring
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yaml
  type: http
slug: ispring-authentication
source_filename: ispring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/authentication/ispring-authentication.yml
summary_line: http · 1 scheme
tags:
- eLearning
- LMS
- Learning Management System
- Training
- Courses
- Enrollments
- Users
- Groups
- Reporting
- Webhooks
- SCORM
- Corporate Training
---
