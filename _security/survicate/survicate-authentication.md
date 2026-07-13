---
api_key_in: []
api_specs:
- filename: survicate-data-export-openapi.yml
  format: yaml
  label: Survicate Data Export API
  slug: survicate-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/survicate/refs/heads/main/openapi/survicate-data-export-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Survicate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Survicate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Survicate
provider_slug: survicate
scheme_count: 1
schemes:
- description: 'Use your Survicate API key as the value for Basic authentication. The API key can be found in the Survicate panel under Surveys Settings > Access Keys. Format: `Basic {{apiKey}}`'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/survicate-data-export-openapi.yml
  type: http
slug: survicate-authentication
source_filename: survicate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/survicate-data-export-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: 'Use your Survicate API key as the value for Basic authentication. The API key\n    can be found in the Survicate panel under Surveys Settings > Access Keys. Format: `Basic\n    {{apiKey}}`'\n  sources:\n  - openapi/survicate-data-export-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/survicate/refs/heads/main/authentication/survicate-authentication.yml
summary_line: http · 1 scheme
tags:
- Surveys
- Customer Feedback
- NPS
- User Research
- Feedback Analytics
- CRM Integration
- Customer Experience
---
