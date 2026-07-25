---
api_key_in: []
api_specs:
- filename: ispring-assignments-api-openapi.yml
  format: yaml
  label: iSpring Learn assignments API
  slug: ispring-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-assignments-api-openapi.yml
- filename: ispring-certificate-api-openapi.yml
  format: yaml
  label: iSpring Learn certificate API
  slug: ispring-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-certificate-api-openapi.yml
- filename: ispring-content-api-openapi.yml
  format: yaml
  label: iSpring Learn content API
  slug: ispring-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-content-api-openapi.yml
- filename: ispring-department-api-openapi.yml
  format: yaml
  label: iSpring Learn department API
  slug: ispring-department-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-department-api-openapi.yml
- filename: ispring-departments-api-openapi.yml
  format: yaml
  label: iSpring Learn departments API
  slug: ispring-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-departments-api-openapi.yml
- filename: ispring-enrollment-api-openapi.yml
  format: yaml
  label: iSpring Learn enrollment API
  slug: ispring-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-enrollment-api-openapi.yml
- filename: ispring-gamification-api-openapi.yml
  format: yaml
  label: iSpring Learn gamification API
  slug: ispring-gamification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-gamification-api-openapi.yml
- filename: ispring-group-api-openapi.yml
  format: yaml
  label: iSpring Learn group API
  slug: ispring-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-group-api-openapi.yml
- filename: ispring-jobtraining-api-openapi.yml
  format: yaml
  label: iSpring Learn jobtraining API
  slug: ispring-jobtraining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-jobtraining-api-openapi.yml
- filename: ispring-learning-track-api-openapi.yml
  format: yaml
  label: iSpring Learn learning_track API
  slug: ispring-learning-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-learning-track-api-openapi.yml
- filename: ispring-performance-management-api-openapi.yml
  format: yaml
  label: iSpring Learn performance-management API
  slug: ispring-performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-performance-management-api-openapi.yml
- filename: ispring-quizzes-api-openapi.yml
  format: yaml
  label: iSpring Learn quizzes API
  slug: ispring-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-quizzes-api-openapi.yml
- filename: ispring-report-api-openapi.yml
  format: yaml
  label: iSpring Learn report API
  slug: ispring-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-report-api-openapi.yml
- filename: ispring-results-api-openapi.yml
  format: yaml
  label: iSpring Learn results API
  slug: ispring-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-results-api-openapi.yml
- filename: ispring-statistics-api-openapi.yml
  format: yaml
  label: iSpring Learn statistics API
  slug: ispring-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-statistics-api-openapi.yml
- filename: ispring-task-api-openapi.yml
  format: yaml
  label: iSpring Learn task API
  slug: ispring-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-task-api-openapi.yml
- filename: ispring-token-api-openapi.yml
  format: yaml
  label: iSpring Learn token API
  slug: ispring-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-token-api-openapi.yml
- filename: ispring-training-api-openapi.yml
  format: yaml
  label: iSpring Learn training API
  slug: ispring-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-training-api-openapi.yml
- filename: ispring-user-api-openapi.yml
  format: yaml
  label: iSpring Learn user API
  slug: ispring-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-user-api-openapi.yml
- filename: ispring-webhook-api-openapi.yml
  format: yaml
  label: iSpring Learn webhook API
  slug: ispring-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-webhook-api-openapi.yml
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
