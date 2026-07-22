---
api_key_in: []
api_specs:
- filename: workstream-public-api-openapi-original.json
  format: json
  label: Workstream Public API
  slug: workstream-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-public-api-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workstream Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Workstream secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Workstream
provider_slug: workstream
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://public-api.workstream.us/
    flow: implicit
    scopes: 10
  name: oauth2
  sources:
  - openapi/workstream-public-api-openapi-original.json
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workstream-public-api-openapi-original.json
  type: http
slug: workstream-authentication
source_filename: workstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/workstream-public-api-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://public-api.workstream.us/\n    scopes: 10\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/authentication/workstream-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Hr Tech
- Hiring
- Payroll
- Onboarding
- Applicant Tracking
- Hourly Workforce
- Restaurants
---
