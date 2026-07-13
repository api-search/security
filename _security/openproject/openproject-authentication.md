---
api_key_in: []
api_specs:
- filename: openproject-openapi.yml
  format: yaml
  label: OpenProject API v3
  slug: openproject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openproject/refs/heads/main/openapi/openproject-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openproject Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenProject secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenProject
provider_slug: openproject
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/openproject-openapi.yml
  type: http
slug: openproject-authentication
source_filename: openproject-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openproject-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/openproject-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openproject/refs/heads/main/authentication/openproject-authentication.yml
summary_line: http · 1 scheme
tags:
- Agile
- Gantt
- Open Source
- Project Management
- Time Tracking
- Work Packages
---
