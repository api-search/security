---
api_key_in:
- query
api_specs:
- filename: tms-onconnect-openapi.yml
  format: yaml
  label: TMS OnConnect API
  slug: tms-onconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tms-onconnect-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tribune Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tribune Media secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tribune Media
provider_slug: tribune-media
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/tms-onconnect-openapi.yml
  type: apiKey
slug: tribune-media-authentication
source_filename: tribune-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tms-onconnect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/tms-onconnect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/authentication/tribune-media-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Media
- Entertainment
- Broadcasting
- Television
- Movies
- Sports
- Celebrity
- Fortune 1000
---
