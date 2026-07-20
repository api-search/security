---
api_key_in: []
api_specs:
- filename: creed-openapi-original.json
  format: json
  label: Creed API
  slug: creed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creed/refs/heads/main/openapi/creed-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Creed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creed secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Creed
provider_slug: creed
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Supabase JWT token
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/creed-openapi-original.json
  type: http
slug: creed-authentication
source_filename: creed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/creed-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Supabase JWT token\n  sources:\n  - openapi/creed-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creed/refs/heads/main/authentication/creed-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Faith
- Religion
- Christianity
- Bible
- Prayer
- Artificial Intelligence
- Chatbot
- Consumer
- Community
---
