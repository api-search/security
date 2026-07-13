---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gracenote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gracenote secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gracenote
provider_slug: gracenote
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/gracenote-openapi.yml
  type: apiKey
slug: gracenote-authentication
source_filename: gracenote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gracenote-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/gracenote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/authentication/gracenote-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Content Metadata
- Entertainment
- Music
- Nielsen
- Sports
- Streaming
- Television
- Video
---
