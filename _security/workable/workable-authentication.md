---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workable
provider_slug: workable
scheme_count: 1
schemes:
- description: 'Workable API token authentication using Bearer token in Authorization header.

    Token types include account tokens, user tokens, and API access tokens.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workable-openapi.yml
  type: http
slug: workable-authentication
source_filename: workable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Workable API token authentication using Bearer token in Authorization header.\n    Token types include account tokens, user tokens, and API access tokens.\n  sources:\n  - openapi/workable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workable/refs/heads/main/authentication/workable-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- ATS
- Recruiting
- Sourcing
- Video Interviews
- Assessments
- SaaS
---
