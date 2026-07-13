---
api_key_in: []
api_specs:
- filename: threads-api-openapi.yml
  format: yaml
  label: Threads API
  slug: threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Threads Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Threads secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Threads
provider_slug: threads-api
scheme_count: 2
schemes:
- name: noauthAuth
  scheme: noauth
  sources:
  - openapi/threads-api-openapi.yml
  - openapi/threads-api.yml
  type: http
- name: oauth2Auth
  scheme: oauth2
  sources:
  - openapi/threads-api-openapi.yml
  - openapi/threads-api.yml
  type: http
slug: threads-api-authentication
source_filename: threads-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/threads-api-openapi.yml, openapi/threads-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: noauthAuth\n  type: http\n  scheme: noauth\n  sources:\n  - openapi/threads-api-openapi.yml\n  - openapi/threads-api.yml\n- name: oauth2Auth\n  type: http\n  scheme: oauth2\n  sources:\n  - openapi/threads-api-openapi.yml\n  - openapi/threads-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/authentication/threads-api-authentication.yml
summary_line: http · 2 schemes
tags:
- Social
- Social Networks
- Meta
- Publishing
- Media
---
