---
api_key_in:
- header
api_specs:
- filename: sendbird-platform-openapi.yml
  format: yaml
  label: Sendbird Platform API
  slug: sendbird-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/openapi/sendbird-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sendbird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sendbird secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sendbird
provider_slug: sendbird
scheme_count: 1
schemes:
- description: Sendbird API token obtained from the Sendbird Dashboard.
  in: header
  name: apiTokenAuth
  parameter: Api-Token
  sources:
  - openapi/sendbird-platform-openapi.yml
  type: apiKey
slug: sendbird-authentication
source_filename: sendbird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sendbird-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Api-Token\n  description: Sendbird API token obtained from the Sendbird Dashboard.\n  sources:\n  - openapi/sendbird-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/authentication/sendbird-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
