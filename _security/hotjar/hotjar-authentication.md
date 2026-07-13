---
api_key_in: []
api_specs:
- filename: hotjar-rest-api-openapi.yml
  format: yaml
  label: Hotjar REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/openapi/hotjar-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hotjar Authentication
name_suffix: Authentication
oauth_flows: []
overview: hotjar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: hotjar
provider_slug: hotjar
scheme_count: 1
schemes:
- description: Bearer token obtained from the OAuth token endpoint using client credentials grant.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hotjar-rest-api-openapi.yml
  type: http
slug: hotjar-authentication
source_filename: hotjar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hotjar-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the OAuth token endpoint using client credentials\n    grant.\n  sources:\n  - openapi/hotjar-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/authentication/hotjar-authentication.yml
summary_line: http · 1 scheme
tags: []
---
