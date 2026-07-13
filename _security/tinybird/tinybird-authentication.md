---
api_key_in: []
api_specs:
- filename: tinybird-openapi.yml
  format: yaml
  label: Tinybird API
  slug: tinybird
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tinybird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tinybird secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tinybird
provider_slug: tinybird
scheme_count: 1
schemes:
- description: Tinybird authentication token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tinybird-openapi.yml
  type: http
slug: tinybird-authentication
source_filename: tinybird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tinybird-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Tinybird authentication token\n  sources:\n  - openapi/tinybird-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/authentication/tinybird-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Data
- Real-Time
- SQL
- Streaming
---
