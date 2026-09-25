---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ispring-assignments-api-openapi.yml
  format: yaml
  label: iSpring Learn Assignments API
  slug: ispring-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-assignments-api-openapi.yml
- filename: ispring-certificate-api-openapi.yml
  format: yaml
  label: iSpring Learn Certificate API
  slug: ispring-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-certificate-api-openapi.yml
- filename: ispring-content-api-openapi.yml
  format: yaml
  label: iSpring Learn Content API
  slug: ispring-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-content-api-openapi.yml
- filename: ispring-department-api-openapi.yml
  format: yaml
  label: iSpring Learn Department API
  slug: ispring-department-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-department-api-openapi.yml
- filename: ispring-departments-api-openapi.yml
  format: yaml
  label: iSpring Learn Departments API
  slug: ispring-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-departments-api-openapi.yml
- filename: ispring-enrollment-api-openapi.yml
  format: yaml
  label: iSpring Learn Enrollment API
  slug: ispring-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-enrollment-api-openapi.yml
- filename: ispring-gamification-api-openapi.yml
  format: yaml
  label: iSpring Learn Gamification API
  slug: ispring-gamification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-gamification-api-openapi.yml
- filename: ispring-group-api-openapi.yml
  format: yaml
  label: iSpring Learn Group API
  slug: ispring-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-group-api-openapi.yml
- filename: ispring-jobtraining-api-openapi.yml
  format: yaml
  label: iSpring Learn Jobtraining API
  slug: ispring-jobtraining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-jobtraining-api-openapi.yml
- filename: ispring-learning-track-api-openapi.yml
  format: yaml
  label: iSpring Learn Learning Track API
  slug: ispring-learning-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-learning-track-api-openapi.yml
- filename: ispring-performance-management-api-openapi.yml
  format: yaml
  label: iSpring Learn Performance Management API
  slug: ispring-performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-performance-management-api-openapi.yml
- filename: ispring-quizzes-api-openapi.yml
  format: yaml
  label: iSpring Learn Quizzes API
  slug: ispring-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-quizzes-api-openapi.yml
- filename: ispring-report-api-openapi.yml
  format: yaml
  label: iSpring Learn Report API
  slug: ispring-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-report-api-openapi.yml
- filename: ispring-results-api-openapi.yml
  format: yaml
  label: iSpring Learn Results API
  slug: ispring-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-results-api-openapi.yml
- filename: ispring-statistics-api-openapi.yml
  format: yaml
  label: iSpring Learn Statistics API
  slug: ispring-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-statistics-api-openapi.yml
- filename: ispring-task-api-openapi.yml
  format: yaml
  label: iSpring Learn Task API
  slug: ispring-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-task-api-openapi.yml
- filename: ispring-token-api-openapi.yml
  format: yaml
  label: iSpring Learn Token API
  slug: ispring-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-token-api-openapi.yml
- filename: ispring-training-api-openapi.yml
  format: yaml
  label: iSpring Learn Training API
  slug: ispring-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-training-api-openapi.yml
- filename: ispring-user-api-openapi.yml
  format: yaml
  label: iSpring Learn User API
  slug: ispring-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-user-api-openapi.yml
- filename: ispring-webhook-api-openapi.yml
  format: yaml
  label: iSpring Learn Webhook API
  slug: ispring-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
- E-Learning
- LMS
- Learning Management System
- Training
- Courses
- Enrollment
- User
- Group
- Reporting
- Webhook
- SCORM
- Corporate Training
---
