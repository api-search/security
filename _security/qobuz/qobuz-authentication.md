---
api_key_in:
- header
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Qobuz Music API
  slug: music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qobuz/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qobuz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qobuz secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qobuz
provider_slug: qobuz
scheme_count: 2
schemes:
- description: Qobuz application identifier issued to partners
  in: query
  name: AppId
  parameter: app_id
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: User authentication token obtained from /user/login
  in: header
  name: UserAuthToken
  parameter: X-User-Auth-Token
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: qobuz-authentication
source_filename: qobuz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: AppId\n  type: apiKey\n  in: query\n  parameter: app_id\n  description: Qobuz application identifier issued to partners\n  sources:\n  - openapi/openapi.yml\n- name: UserAuthToken\n  type: apiKey\n  in: header\n  parameter: X-User-Auth-Token\n  description: User authentication token obtained from /user/login\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qobuz/refs/heads/main/authentication/qobuz-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Music Streaming
- Hi-Res Audio
- FLAC
- Lossless Audio
- Music Downloads
- Catalog Search
- Streaming URLs
- Music Metadata
- Audiophile
- France
---
