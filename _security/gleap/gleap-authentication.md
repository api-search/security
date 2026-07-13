---
api_key_in: []
api_specs:
- filename: api-docs.json
  format: json
  label: Gleap REST API
  slug: gleap-rest-api
  spec_type: OpenAPI
  url: https://api.gleap.io/api-docs.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gleap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gleap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gleap
provider_slug: gleap
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/gleap-rest-api-openapi.yml
  type: http
slug: gleap-authentication
source_filename: gleap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gleap-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/gleap-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gleap/refs/heads/main/authentication/gleap-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Feedback
- Bug Reporting
- In-App Support
- Feature Requests
- Roadmap
- Live Chat
- AI Agents
- Session Replay
- Help Center
- Ticketing
- User Feedback
- SaaS
---
