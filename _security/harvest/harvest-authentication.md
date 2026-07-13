---
api_key_in: []
api_specs:
- filename: harvest-openapi.yml
  format: yaml
  label: Harvest API v2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harvest/refs/heads/main/openapi/harvest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Harvest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harvest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harvest
provider_slug: harvest
scheme_count: 1
schemes:
- description: 'Personal access token or OAuth 2.0 access token passed in the

    Authorization header. The Harvest-Account-Id header (or account_id

    query parameter) is also required.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/harvest-openapi.yml
  type: http
slug: harvest-authentication
source_filename: harvest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harvest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Personal access token or OAuth 2.0 access token passed in the\n    Authorization header. The Harvest-Account-Id header (or account_id\n    query parameter) is also required.\n  sources:\n  - openapi/harvest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harvest/refs/heads/main/authentication/harvest-authentication.yml
summary_line: http · 1 scheme
tags:
- Time Tracking
- Project Management
- Invoicing
- Expense Tracking
- Timesheets
- Professional Services
---
