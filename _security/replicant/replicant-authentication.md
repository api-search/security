---
api_key_in: []
api_specs:
- filename: replicant-replicant-api-openapi.yml
  format: yaml
  label: Replicant Replicant API
  slug: replicant-replicant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicant/refs/heads/main/openapi/replicant-replicant-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Replicant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Replicant
provider_slug: replicant
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/replicant-outbound-api-openapi.yml
  type: http
slug: replicant-authentication
source_filename: replicant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/replicant-outbound-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/replicant-outbound-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicant/refs/heads/main/authentication/replicant-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Contact Center
- Conversational AI
- Customer Service
- Voice AI
- Contact Center Automation
- Agentic AI
- Conversation Intelligence
---
