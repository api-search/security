---
api_key_in:
- header
api_specs:
- filename: 2sAY548Kou
  format: yaml
  label: TalentLMS API
  slug: talentlms-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/31867199/2sAY548Kou
- filename: talentlms-batch-actions-api-openapi.yml
  format: yaml
  label: TalentLMS Batch Actions API
  slug: talentlms-batch-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-batch-actions-api-openapi.yml
- filename: talentlms-branch-api-openapi.yml
  format: yaml
  label: TalentLMS Branch API
  slug: talentlms-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-branch-api-openapi.yml
- filename: talentlms-category-api-openapi.yml
  format: yaml
  label: TalentLMS Category API
  slug: talentlms-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-category-api-openapi.yml
- filename: talentlms-course-api-openapi.yml
  format: yaml
  label: TalentLMS Course API
  slug: talentlms-course-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-course-api-openapi.yml
- filename: talentlms-group-api-openapi.yml
  format: yaml
  label: TalentLMS Group API
  slug: talentlms-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-group-api-openapi.yml
- filename: talentlms-learning-paths-api-openapi.yml
  format: yaml
  label: TalentLMS Learning Paths API
  slug: talentlms-learning-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-learning-paths-api-openapi.yml
- filename: talentlms-portal-api-openapi.yml
  format: yaml
  label: TalentLMS Portal API
  slug: talentlms-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-portal-api-openapi.yml
- filename: talentlms-task-api-openapi.yml
  format: yaml
  label: TalentLMS Task API
  slug: talentlms-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-task-api-openapi.yml
- filename: talentlms-timeline-api-openapi.yml
  format: yaml
  label: TalentLMS Timeline API
  slug: talentlms-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-timeline-api-openapi.yml
- filename: talentlms-unit-api-openapi.yml
  format: yaml
  label: TalentLMS Unit API
  slug: talentlms-unit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-unit-api-openapi.yml
- filename: talentlms-user-api-openapi.yml
  format: yaml
  label: TalentLMS User API
  slug: talentlms-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Talentlms Authentication
name_suffix: Authentication
oauth_flows: []
overview: TalentLMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TalentLMS
provider_slug: talentlms
scheme_count: 1
schemes:
- in: header
  name: apikeyAuth
  parameter: X-API-Key
  sources:
  - openapi/talentlms-openapi.yaml
  type: apiKey
slug: talentlms-authentication
source_filename: talentlms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/talentlms-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/talentlms-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/authentication/talentlms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Learning Management System
- LMS
- eLearning
- Training
- Courses
- Users
- Enrollments
- Education
- HR Tech
- Cloud
---
