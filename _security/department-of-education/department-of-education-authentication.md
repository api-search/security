---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Department Of Education Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Education secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Education
provider_slug: department-of-education
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/department-of-education-openapi.yml
  type: apiKey
slug: department-of-education-authentication
source_filename: department-of-education-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/department-of-education-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/department-of-education-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-education/refs/heads/main/authentication/department-of-education-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- College Scorecard
- Education
- Federal Government
- Higher Education
- IPEDS
- K-12
- NCES
- Open Data
- Postsecondary
---
