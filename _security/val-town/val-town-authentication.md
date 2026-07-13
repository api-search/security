---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Val Town REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.val.town/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Val Town Authentication
name_suffix: Authentication
oauth_flows: []
overview: Val Town secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Val Town
provider_slug: val-town
scheme_count: 1
schemes:
- description: Endpoints that support authorization expect Bearer authentication, using an API token provided from Val Town.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/val-town-rest-api-openapi.yml
  type: http
slug: val-town-authentication
source_filename: val-town-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/val-town-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Endpoints that support authorization expect Bearer authentication, using an API\n    token provided from Val Town.\n  sources:\n  - openapi/val-town-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/authentication/val-town-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Serverless
- JavaScript
- TypeScript
- Social Coding
- HTTP Endpoints
- Cron Jobs
- Email
- SQLite
- Blob Storage
---
