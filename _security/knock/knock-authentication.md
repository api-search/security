---
api_key_in: []
api_specs:
- filename: knock-openapi.json
  format: json
  label: Knock Workflows API
  slug: knock-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Messages API
  slug: knock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Users API
  slug: knock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Objects API
  slug: knock-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Feeds API
  slug: knock-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Guides API
  slug: knock-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Schedules API
  slug: knock-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Preferences API
  slug: knock-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Knock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knock
provider_slug: knock
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/knock-openapi.json
  type: http
slug: knock-authentication
source_filename: knock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knock-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/knock-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/authentication/knock-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Email
- SMS
- Push
- Workflows
---
