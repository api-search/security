---
api_key_in: []
api_specs:
- filename: openverse-audio-api-openapi.yml
  format: yaml
  label: Openverse audio API
  slug: openverse-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/openapi/openverse-audio-api-openapi.yml
- filename: openverse-auth-api-openapi.yml
  format: yaml
  label: Openverse auth API
  slug: openverse-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/openapi/openverse-auth-api-openapi.yml
- filename: openverse-images-api-openapi.yml
  format: yaml
  label: Openverse images API
  slug: openverse-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/openapi/openverse-images-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openverse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openverse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Openverse
provider_slug: openverse
scheme_count: 1
schemes:
- name: Openverse API Token
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: openverse-authentication
source_filename: openverse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Openverse API Token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/authentication/openverse-authentication.yml
summary_line: http · 1 scheme
tags:
- Images
- Audio
- Creative Commons
- Open Media
- Search
- Open Data
- Cultural Heritage
- Museums
---
