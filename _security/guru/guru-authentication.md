---
api_key_in: []
api_specs:
- filename: guru-openapi.yml
  format: yaml
  label: Guru REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Guru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guru secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Guru
provider_slug: guru
scheme_count: 2
schemes:
- description: API token authentication via HTTP Basic.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/guru-openapi.yml
  type: http
- description: OAuth 2.0 bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/guru-openapi.yml
  type: http
slug: guru-authentication
source_filename: guru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guru-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API token authentication via HTTP Basic.\n  sources:\n  - openapi/guru-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token.\n  sources:\n  - openapi/guru-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/authentication/guru-authentication.yml
summary_line: http · 2 schemes
tags:
- Knowledge Management
- Enterprise Search
- AI Knowledge Base
- Internal Wiki
- Verified Knowledge
- Workplace Productivity
---
