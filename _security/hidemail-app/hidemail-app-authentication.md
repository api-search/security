---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hidemail-app-endpoints-api-openapi.yml
  format: yaml
  label: HideMail Endpoints API
  slug: hidemail-app-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hidemail-app/openapi/hidemail-app-endpoints-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: HideMail Authentication
name_suffix: Authentication
oauth_flows: []
overview: HideMail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HideMail
provider_slug: hidemail-app
scheme_count: 1
schemes:
- description: You can retrieve your token by visiting your dashboard, find in menu <b>API tokens</b> and create a new one.
  name: default
  scheme: bearer
  sources:
  - openapi/hidemail-app-openapi.yml
  - openapi/openapi.yaml
  type: http
slug: hidemail-app-authentication
source_filename: hidemail-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hidemail-app-openapi.yml, openapi/openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: default\n  type: http\n  scheme: bearer\n  description: You can retrieve your token by visiting your dashboard, find in menu <b>API tokens</b>\n    and create a new one.\n  sources:\n  - openapi/hidemail-app-openapi.yml\n  - openapi/openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/hidemail-app/authentication/hidemail-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email
- Privacy
- Alias
- Software-as-a-Service
- Free
---
