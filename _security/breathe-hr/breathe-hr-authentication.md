---
api_key_in:
- header
api_specs:
- filename: breathe-hr-openapi.yml
  format: yaml
  label: Breathe HR REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breathe-hr/refs/heads/main/openapi/breathe-hr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Breathe Hr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breathe HR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Breathe HR
provider_slug: breathe-hr
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/breathe-hr-openapi.yml
  type: apiKey
slug: breathe-hr-authentication
source_filename: breathe-hr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/breathe-hr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/breathe-hr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breathe-hr/refs/heads/main/authentication/breathe-hr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- HR
- HRIS
- Human Resources
- Employee Management
- Absence Management
- Holiday Tracking
- SMB
- UK
---
