---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hibob Authentication
name_suffix: Authentication
oauth_flows: []
overview: HiBob secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HiBob
provider_slug: hibob
scheme_count: 1
schemes:
- description: Service user credentials passed via HTTP Basic Authorization header
  name: serviceUserAuth
  scheme: basic
  sources:
  - openapi/hibob-openapi.yml
  type: http
slug: hibob-authentication
source_filename: hibob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hibob-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: serviceUserAuth\n  type: http\n  scheme: basic\n  description: Service user credentials passed via HTTP Basic Authorization header\n  sources:\n  - openapi/hibob-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/authentication/hibob-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- HRIS
- People Operations
- Employee Data
- Time Off
- HR Tech
---
