---
api_key_in: []
api_specs:
- filename: powerschool-authentication-api-openapi.yml
  format: yaml
  label: PowerSchool Authentication API
  slug: powerschool-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-authentication-api-openapi.yml
- filename: powerschool-courses-api-openapi.yml
  format: yaml
  label: PowerSchool Courses API
  slug: powerschool-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-courses-api-openapi.yml
- filename: powerschool-district-api-openapi.yml
  format: yaml
  label: PowerSchool District API
  slug: powerschool-district-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-district-api-openapi.yml
- filename: powerschool-metadata-api-openapi.yml
  format: yaml
  label: PowerSchool Metadata API
  slug: powerschool-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-metadata-api-openapi.yml
- filename: powerschool-powerquery-api-openapi.yml
  format: yaml
  label: PowerSchool PowerQuery API
  slug: powerschool-powerquery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-powerquery-api-openapi.yml
- filename: powerschool-schools-api-openapi.yml
  format: yaml
  label: PowerSchool Schools API
  slug: powerschool-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-schools-api-openapi.yml
- filename: powerschool-sections-api-openapi.yml
  format: yaml
  label: PowerSchool Sections API
  slug: powerschool-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-sections-api-openapi.yml
- filename: powerschool-students-api-openapi.yml
  format: yaml
  label: PowerSchool Students API
  slug: powerschool-students-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-students-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Powerschool Authentication
name_suffix: Authentication
oauth_flows: []
overview: PowerSchool secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PowerSchool
provider_slug: powerschool
scheme_count: 2
schemes:
- description: Bearer token obtained from /oauth/access_token/ using client credentials. Tokens expire and must be refreshed.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/powerschool-powerschool-sis-api-openapi.yml
  type: http
- description: Basic auth with Base64-encoded client_id:client_secret for the token endpoint only.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/powerschool-powerschool-sis-api-openapi.yml
  type: http
slug: powerschool-authentication
source_filename: powerschool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/powerschool-powerschool-sis-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from /oauth/access_token/ using client credentials. Tokens\n    expire and must be refreshed.\n  sources:\n  - openapi/powerschool-powerschool-sis-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic auth with Base64-encoded client_id:client_secret for the token endpoint\n    only.\n  sources:\n  - openapi/powerschool-powerschool-sis-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/authentication/powerschool-authentication.yml
summary_line: http · 2 schemes
tags:
- K-12
- Education
- Student Information System
- SIS
- Students
- Grades
- Attendance
- Enrollment
- Scheduling
- EdTech
---
