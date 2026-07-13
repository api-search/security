---
api_key_in: []
api_specs:
- filename: qualcomm-qualcomm-api-openapi.yml
  format: yaml
  label: Qualcomm Developer API
  slug: qualcomm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualcomm/refs/heads/main/openapi/qualcomm-qualcomm-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qualcomm Authentication
name_suffix: Authentication
oauth_flows: []
overview: qualcomm secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: qualcomm
provider_slug: qualcomm
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qualcomm-qualcomm-api-openapi.yml
  type: http
slug: qualcomm-authentication
source_filename: qualcomm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qualcomm-qualcomm-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/qualcomm-qualcomm-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualcomm/refs/heads/main/authentication/qualcomm-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 500
---
