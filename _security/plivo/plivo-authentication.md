---
api_key_in: []
api_specs:
- filename: plivo-asyncapi.yml
  format: yaml
  label: Plivo Audio Stream API
  slug: plivo-audio-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/plivo/refs/heads/main/asyncapi/plivo-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Plivo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plivo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plivo
provider_slug: plivo
scheme_count: 1
schemes:
- description: HTTP Basic with Plivo Auth ID (username) and Auth Token (password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/plivo-openapi.yml
  type: http
slug: plivo-authentication
source_filename: plivo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plivo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with Plivo Auth ID (username) and Auth Token (password).\n  sources:\n  - openapi/plivo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plivo/refs/heads/main/authentication/plivo-authentication.yml
summary_line: http · 1 scheme
tags:
- Communications
- CPaaS
- Voice
- SMS
- Messaging
- WhatsApp
- SIP Trunking
- Verify
---
