---
api_key_in: []
api_specs:
- filename: tvdb-openapi.yml
  format: yaml
  label: TheTVDB v4 API
  slug: tvdb-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/openapi/tvdb-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tvdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheTVDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TheTVDB
provider_slug: tvdb
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tvdb-openapi.yml
  type: http
slug: tvdb-authentication
source_filename: tvdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tvdb-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tvdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/authentication/tvdb-authentication.yml
summary_line: http · 1 scheme
tags:
- Entertainment
- Movies
- Television
- Media Metadata
- Public APIs
- Video
---
