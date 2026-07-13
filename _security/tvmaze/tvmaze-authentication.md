---
api_key_in: []
api_specs:
- filename: tvmaze-public-openapi.yml
  format: yaml
  label: TVmaze Public API
  slug: tvmaze-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-public-openapi.yml
- filename: tvmaze-premium-openapi.yml
  format: yaml
  label: TVmaze Premium User API
  slug: tvmaze-premium-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-premium-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tvmaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: TVmaze secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TVmaze
provider_slug: tvmaze
scheme_count: 1
schemes:
- name: usertoken
  scheme: basic
  sources:
  - openapi/tvmaze-premium-openapi.yml
  type: http
slug: tvmaze-authentication
source_filename: tvmaze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tvmaze-premium-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: usertoken\n  type: http\n  scheme: basic\n  sources:\n  - openapi/tvmaze-premium-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/authentication/tvmaze-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Television
- Streaming
- Schedule
- Metadata
- Entertainment
- Public APIs
---
