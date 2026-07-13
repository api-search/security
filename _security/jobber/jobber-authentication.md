---
api_key_in: []
api_specs:
- filename: jobber-developer-api-openapi.yml
  format: yaml
  label: Jobber Developer API
  slug: jobber-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/openapi/jobber-developer-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jobber Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jobber secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jobber
provider_slug: jobber
scheme_count: 1
schemes:
- bearerFormat: OAuth 2.0 Access Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jobber-developer-api-openapi.yml
  type: http
slug: jobber-authentication
source_filename: jobber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jobber-developer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.0 Access Token\n  sources:\n  - openapi/jobber-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/authentication/jobber-authentication.yml
summary_line: http · 1 scheme
tags:
- Field Service Management
- Home Service
- Scheduling
- Quoting
- Invoicing
- Dispatching
- Mobile Workforce
- CRM
- SaaS
- GraphQL
---
