---
api_key_in: []
api_specs:
- filename: squadcast-openapi.yml
  format: yaml
  label: Squadcast Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squadcast/refs/heads/main/openapi/squadcast-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Squadcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Squadcast secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Squadcast
provider_slug: squadcast
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer access token obtained via the `/oauth/access-token` endpoint on

    the auth host. Send as `Authorization: Bearer <access_token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/squadcast-openapi.yml
  type: http
slug: squadcast-authentication
source_filename: squadcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/squadcast-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Bearer access token obtained via the `/oauth/access-token` endpoint on\n    the auth host. Send as `Authorization: Bearer <access_token>`.\n  sources:\n  - openapi/squadcast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squadcast/refs/heads/main/authentication/squadcast-authentication.yml
summary_line: http · 1 scheme
tags:
- Incident Response
- On-Call Management
- DevOps
- SRE
- Alerting
- Incident Management
---
