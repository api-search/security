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
name: knowsme Authentication
name_suffix: Authentication
oauth_flows: []
overview: knowsme secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: knowsme
provider_slug: knowsme-dev
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/knowsme-dev-openapi.yml
  type: http
slug: knowsme-dev-authentication
source_filename: knowsme-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/knowsme-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/knowsme-dev-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/knowsme-dev/authentication/knowsme-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Memory
- Privacy
- Ghana
---
