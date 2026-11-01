---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Alexishr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alexis secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alexis
provider_slug: alexishr
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/alexishr-openapi.json
  type: http
slug: alexishr-authentication
source_filename: alexishr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/alexishr-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/alexishr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/alexishr/authentication/alexishr-authentication.yml
summary_line: http · 1 scheme
tags:
- People Analytics
- Payroll
- AI Chatbot
- Integrations
- Onboarding
- Performance Management
- User Provisioning
---
