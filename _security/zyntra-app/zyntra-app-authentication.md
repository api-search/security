---
anonymous_access: false
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zyntra App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zyntra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zyntra
provider_slug: zyntra-app
scheme_count: 1
schemes:
- in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/zyntra-app-openapi.yml
  type: apiKey
slug: zyntra-app-authentication
source_filename: zyntra-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/zyntra-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/zyntra-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/zyntra-app/authentication/zyntra-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Testing
- Automated Tests
- QA
- Password Reset
- Magic Link
---
