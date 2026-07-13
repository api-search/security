---
api_key_in: []
api_specs:
- filename: intralinks-api-openapi.yml
  format: yaml
  label: Intralinks API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Intralinks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intralinks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intralinks
provider_slug: intralinks
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token obtained from the /oauth/token endpoint. Pass the token in the Authorization header as 'Bearer {token}'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/intralinks-api-openapi.yml
  type: http
slug: intralinks-authentication
source_filename: intralinks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/intralinks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained from the /oauth/token endpoint. Pass the token\n    in the Authorization header as 'Bearer {token}'.\n  sources:\n  - openapi/intralinks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/authentication/intralinks-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
---
