---
api_key_in:
- header
api_specs:
- filename: soundstripe-openapi.yml
  format: yaml
  label: Soundstripe API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Soundstripe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soundstripe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soundstripe
provider_slug: soundstripe
scheme_count: 1
schemes:
- description: 'Token authentication. Send `Authorization: Token <api-key>`. Keys are privileged — server-to-server use only, never from client-side code.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/soundstripe-openapi.yml
  type: apiKey
slug: soundstripe-authentication
source_filename: soundstripe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soundstripe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token authentication. Send `Authorization: Token <api-key>`. Keys are privileged\n    — server-to-server use only, never from client-side code.'\n  sources:\n  - openapi/soundstripe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/authentication/soundstripe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Music
- Sound Effects
- Stock Video
- Royalty Free
- Licensing
- Subscription
- Creators
- Content Creation
- Video Production
- Podcasting
- AI Music Supervisor
- Stems
---
