---
api_key_in: []
api_specs:
- filename: import2-openapi.yml
  format: yaml
  label: Import2 API
  slug: import2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/import2/refs/heads/main/openapi/import2-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Import2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Import2 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Import2
provider_slug: import2
scheme_count: 1
schemes:
- description: 'HTTP Basic Authentication. Supply the API token as the username and any value (e.g. "X") as the password. Example: curl -u <api_token>:X.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/import2-openapi.yml
  type: http
slug: import2-authentication
source_filename: import2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/import2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic Authentication. Supply the API token as the username and any value\n    (e.g. \"X\") as the password. Example: curl -u <api_token>:X.'\n  sources:\n  - openapi/import2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/import2/refs/heads/main/authentication/import2-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Migration
- Data Integration
- CRM
- Helpdesk
- SaaS
- Migration
- Onboarding
---
