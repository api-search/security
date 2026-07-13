---
api_key_in:
- header
api_specs:
- filename: messaging-api-openapi.yml
  format: yaml
  label: Messaging API Messages API
  slug: messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messaging-api/refs/heads/main/openapi/messaging-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Messaging Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Messaging API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Messaging API
provider_slug: messaging-api
scheme_count: 1
schemes:
- in: header
  name: apiKeys
  parameter: api-key
  sources:
  - openapi/messaging-api-openapi.yml
  type: apiKey
slug: messaging-api-authentication
source_filename: messaging-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/messaging-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeys\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/messaging-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messaging-api/refs/heads/main/authentication/messaging-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Pattern
- Messaging
- Template
---
