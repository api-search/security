---
api_key_in: []
api_specs:
- filename: western-digital-my-cloud-home-openapi.yml
  format: yaml
  label: WD My Cloud Home API
  slug: my-cloud-home
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-my-cloud-home-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Western Digital Authentication
name_suffix: Authentication
oauth_flows: []
overview: western-digital secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: western-digital
provider_slug: western-digital
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained via the /oauth/token endpoint. Include in Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/western-digital-my-cloud-home-openapi.yml
  type: http
slug: western-digital-authentication
source_filename: western-digital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/western-digital-my-cloud-home-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained via the /oauth/token endpoint. Include in Authorization\n    header as \"Bearer {token}\".\n  sources:\n  - openapi/western-digital-my-cloud-home-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/authentication/western-digital-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 500
---
