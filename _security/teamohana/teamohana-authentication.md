---
api_key_in:
- header
api_specs:
- filename: teamohana-openapi-original.json
  format: json
  label: TeamOhana Public API
  slug: teamohana-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/openapi/teamohana-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Teamohana Authentication
name_suffix: Authentication
oauth_flows: []
overview: TeamOhana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TeamOhana
provider_slug: teamohana
scheme_count: 1
schemes:
- bearer_format: api-key
  name: Authorization
  scheme: bearer
  sources:
  - openapi/teamohana-openapi-original.json
  type: http
slug: teamohana-authentication
source_filename: teamohana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/teamohana-openapi-original.json\ndocs: https://api.teamohana.us/faq/index.html\nnotes: >-\n  Bearer token authentication via the Authorization header\n  (`Authorization: Bearer YOUR_API_KEY`). Per the API FAQ, the SCIM API and the\n  Headcount API use SEPARATE API keys — ensure the correct key is used for each\n  surface. Keys are provisioned by TeamOhana; contact support to obtain them.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  bearer_format: api-key\n  sources:\n  - openapi/teamohana-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/authentication/teamohana-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Hr Tech
- Headcount Management
- Headcount Planning
- Workforce Planning
- Human Resources
- Talent Acquisition
- Finance
- SCIM
- SaaS
---
