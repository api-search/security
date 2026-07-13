---
api_key_in: []
api_specs:
- filename: api-spec.json
  format: json
  label: Mux Video API
  slug: video-api
  spec_type: OpenAPI
  url: https://www.mux.com/api-spec.json
- filename: api-spec.json
  format: json
  label: Mux Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://www.mux.com/api-spec.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mux Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mux secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mux
provider_slug: mux
scheme_count: 1
schemes:
- description: HTTP Basic auth using a Mux Access Token ID (username) and Secret (password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mux-openapi.yml
  type: http
slug: mux-authentication
source_filename: mux-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mux-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using a Mux Access Token ID (username) and Secret (password).\n  sources:\n  - openapi/mux-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mux/refs/heads/main/authentication/mux-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Live Streaming
- Video Analytics
- QoE
- Video On Demand
- Transcoding
- Mux Player
---
