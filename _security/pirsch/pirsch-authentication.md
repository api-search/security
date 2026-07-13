---
api_key_in: []
api_specs:
- filename: pirsch-pirsch-api-openapi.yml
  format: yaml
  label: Pirsch API
  slug: pirsch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-pirsch-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pirsch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pirsch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pirsch
provider_slug: pirsch
scheme_count: 1
schemes:
- description: Pass an OAuth2 access token obtained from POST /token, or a static access key, as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pirsch-pirsch-api-openapi.yml
  type: http
slug: pirsch-authentication
source_filename: pirsch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pirsch-pirsch-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Pass an OAuth2 access token obtained from POST /token, or a static access key,\n    as a Bearer token in the Authorization header.\n  sources:\n  - openapi/pirsch-pirsch-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/authentication/pirsch-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Web Analytics
- Privacy
- GDPR
- Cookie-Free
- Page Views
- Sessions
- Events
- Conversion Goals
- Funnels
- Traffic Sources
---
