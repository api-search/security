---
api_key_in:
- header
api_specs:
- filename: callrail-openapi.yml
  format: yaml
  label: CallRail v3 API
  slug: v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/openapi/callrail-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Callrail Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallRail secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CallRail
provider_slug: callrail
scheme_count: 1
schemes:
- description: 'Send as `Authorization: Token token="YOUR_API_KEY"`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/callrail-openapi.yml
  type: apiKey
slug: callrail-authentication
source_filename: callrail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/callrail-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Send as `Authorization: Token token=\"YOUR_API_KEY\"`.'\n  sources:\n  - openapi/callrail-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/authentication/callrail-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Call Tracking
- Conversation Intelligence
- Marketing Attribution
- Lead Tracking
- Telephony
- Analytics
- Form Tracking
---
