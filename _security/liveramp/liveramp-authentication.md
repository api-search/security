---
api_key_in: []
api_specs:
- filename: liveramp-openapi.yml
  format: yaml
  label: LiveRamp Activation API
  slug: activation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Liveramp Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiveRamp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LiveRamp
provider_slug: liveramp
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token obtained from the LiveRamp service account token URI; passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/liveramp-openapi.yml
  type: http
slug: liveramp-authentication
source_filename: liveramp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/liveramp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 access token obtained from the LiveRamp service account token URI;\n    passed as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/liveramp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/authentication/liveramp-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Connectivity
- Identity Resolution
- Activation
- Clean Room
- Privacy
- AdTech
---
