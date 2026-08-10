---
api_key_in: []
api_specs:
- filename: songtradr-allowed-values-api-openapi.yml
  format: yaml
  label: Songtradr Allowed Values API
  slug: songtradr-allowed-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-allowed-values-api-openapi.yml
- filename: songtradr-similarity-vector-controller-api-openapi.yml
  format: yaml
  label: Songtradr Similarity Vector Controller API
  slug: songtradr-similarity-vector-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-similarity-vector-controller-api-openapi.yml
- filename: songtradr-user-api-openapi.yml
  format: yaml
  label: Songtradr User API
  slug: songtradr-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Songtradr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Songtradr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Songtradr
provider_slug: songtradr
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: "To authenticate, you have to call POST https://api.songtradr.com/api/v1/user/login \nand use the response's jwtToken as a bearer Token in all following API calls."
  name: bearer-jwt
  scheme: bearer
  sources:
  - openapi/songtradr-api-openapi.yml
  type: http
slug: songtradr-authentication
source_filename: songtradr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/songtradr-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"To authenticate, you have to call POST https://api.songtradr.com/api/v1/user/login\\\n    \\ \\nand use the response's jwtToken as a bearer Token in all following API calls.\"\n  sources:\n  - openapi/songtradr-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/authentication/songtradr-authentication.yml
summary_line: http · 1 scheme
tags:
- music
- music-licensing
- sync-licensing
- music-metadata
- audio-tagging
- semantic-search
- machine-learning
- media
- entertainment
- rights-management
- audio
---
