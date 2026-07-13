---
api_key_in: []
api_specs:
- filename: api-reference
  format: yaml
  label: Argyle API
  slug: argyle-api
  spec_type: OpenAPI
  url: https://docs.argyle.com/api-reference
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Argyle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argyle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argyle
provider_slug: argyle
scheme_count: 1
schemes:
- description: Username = api_key_id, Password = api_key_secret
  name: basicAuth
  scheme: basic
  sources:
  - openapi/argyle-api-openapi.yml
  type: http
slug: argyle-authentication
source_filename: argyle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argyle-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username = api_key_id, Password = api_key_secret\n  sources:\n  - openapi/argyle-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argyle/refs/heads/main/authentication/argyle-authentication.yml
summary_line: http · 1 scheme
tags:
- Employment Data
- Payroll
- Income Verification
- Gig Economy
- Financial Data
- Employment History
- Earned Wage Access
- Direct Deposit
---
