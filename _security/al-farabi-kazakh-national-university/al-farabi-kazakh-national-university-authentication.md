---
api_key_in: []
api_specs:
- filename: al-farabi-kazakh-national-university-open-edx.yaml
  format: yaml
  label: KazNU Open edX API
  slug: kaznu-open-edx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/al-farabi-kazakh-national-university/refs/heads/main/openapi/al-farabi-kazakh-national-university-open-edx.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Al Farabi Kazakh National University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Al-Farabi Kazakh National University secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Al-Farabi Kazakh National University
provider_slug: al-farabi-kazakh-national-university
scheme_count: 1
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/al-farabi-kazakh-national-university-open-edx.yaml
  type: http
slug: al-farabi-kazakh-national-university-authentication
source_filename: al-farabi-kazakh-national-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/al-farabi-kazakh-national-university-open-edx.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/al-farabi-kazakh-national-university-open-edx.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/al-farabi-kazakh-national-university/refs/heads/main/authentication/al-farabi-kazakh-national-university-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Education
- Kazakhstan
- Central Asia
---
