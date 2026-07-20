---
api_key_in: []
api_specs:
- filename: cello-openapi-original.json
  format: json
  label: Cello API
  slug: cello-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cello Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cello secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cello
provider_slug: cello
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cello-openapi-original.json
  type: http
slug: cello-authentication
source_filename: cello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cello-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cello-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/authentication/cello-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Referral Marketing
- Affiliate Marketing
- Growth
- SaaS
- Attribution
- Partner Programs
- Ai Enterprise Software
---
