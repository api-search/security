---
api_key_in: []
api_specs:
- filename: slide-openapi-original.json
  format: json
  label: Slide API
  slug: slide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Slide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slide secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slide
provider_slug: slide
scheme_count: 1
schemes:
- bearerFormat: string
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/slide-openapi-original.json
  token_source: Slide Console (user-scoped API tokens)
  type: http
slug: slide-authentication
source_filename: slide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/slide-openapi-original.json\ndocs: https://docs.slide.tech/api/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Slide authenticates every request with a static Bearer API token supplied in\n  the Authorization header (Authorization: Bearer YOUR_SECRET_TOKEN). Tokens are\n  created and managed in the Slide Console; they are user-based and inherit the\n  role and permissions of the user that created them. There is no OAuth flow and\n  no scope system.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  token_source: Slide Console (user-scoped API tokens)\n  sources:\n  - openapi/slide-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/authentication/slide-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Backup
- Disaster Recovery
- Business Continuity
- BCDR
- Managed Service Providers
- MSP
- Data Protection
- Cloud Storage
- Virtualization
---
