---
api_key_in:
- header
api_specs:
- filename: talentlms-openapi.yaml
  format: yaml
  label: TalentLMS API
  slug: talentlms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-openapi.yaml
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
