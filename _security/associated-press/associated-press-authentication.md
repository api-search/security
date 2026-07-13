---
api_key_in:
- header
- query
api_specs:
- filename: associated-press-meda-openapi-original.yml
  format: yaml
  label: AP Media API
  slug: ap-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/associated-press/refs/heads/main/openapi/associated-press-meda-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Associated Press Authentication
name_suffix: Authentication
oauth_flows: []
overview: Associated Press secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Associated Press
provider_slug: associated-press
scheme_count: 2
schemes:
- description: apikey submitted in HTTP header x-api-key
  in: header
  name: apikey
  parameter: x-api-key
  sources:
  - openapi/associated-press-meda-openapi-original.yml
  type: apiKey
- description: DEPRECATED - no longer supported
  in: query
  name: apikeyUrl
  parameter: apikey
  sources:
  - openapi/associated-press-meda-openapi-original.yml
  type: apiKey
slug: associated-press-authentication
source_filename: associated-press-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/associated-press-meda-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: apikey submitted in HTTP header x-api-key\n  sources:\n  - openapi/associated-press-meda-openapi-original.yml\n- name: apikeyUrl\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: DEPRECATED - no longer supported\n  sources:\n  - openapi/associated-press-meda-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/associated-press/refs/heads/main/authentication/associated-press-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Elections
- Journalism
- Media
- News
- Content
---
