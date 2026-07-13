---
api_key_in:
- header
api_specs:
- filename: free-law-project-openapi.yml
  format: yaml
  label: Free Law Project API
  slug: free-law-project
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Free Law Project Authentication
name_suffix: Authentication
oauth_flows: []
overview: Free Law Project secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Free Law Project
provider_slug: free-law-project
scheme_count: 1
schemes:
- description: 'HTTP token authentication. Format: `Token <your-token>`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/free-law-project-openapi.yml
  type: apiKey
slug: free-law-project-authentication
source_filename: free-law-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/free-law-project-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'HTTP token authentication. Format: `Token <your-token>`.'\n  sources:\n  - openapi/free-law-project-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/authentication/free-law-project-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Courts
- Justice
- Legal
- Transparency
---
