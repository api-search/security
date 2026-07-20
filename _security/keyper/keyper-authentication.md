---
api_key_in:
- header
api_specs:
- filename: keyper-access-openapi.yml
  format: yaml
  label: keyper Access API
  slug: keyper-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keyper/refs/heads/main/openapi/keyper-access-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Keyper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keyper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keyper
provider_slug: keyper
scheme_count: 1
schemes:
- description: "The Authorization header carries either an application secret or a user authentication token. Two documented forms:\n  - \"Authorization: APPSECRET <secret>\"   (string app secret)\n  - \"Authorization: AUTHTOKEN <guid>\"     (per-user authentication token)"
  forms:
  - example_shape: APPSECRET <string>
    kind: app-secret
    prefix: APPSECRET
  - example_shape: AUTHTOKEN <guid>
    kind: auth-token
    prefix: AUTHTOKEN
  header: Authorization
  in: header
  name: keyperAuth
  sources:
  - openapi/keyper-access-openapi.yml
  type: apiKey
slug: keyper-authentication
source_filename: keyper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/keyper/keyper-access-api/blob/master/apiary.apib\ndocs: https://developers.keyper.com\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: keyperAuth\n  type: apiKey\n  in: header\n  header: Authorization\n  description: >-\n    The Authorization header carries either an application secret or a user\n    authentication token. Two documented forms:\n      - \"Authorization: APPSECRET <secret>\"   (string app secret)\n      - \"Authorization: AUTHTOKEN <guid>\"     (per-user authentication token)\n  forms:\n  - kind: app-secret\n    prefix: APPSECRET\n    example_shape: \"APPSECRET <string>\"\n  - kind: auth-token\n    prefix: AUTHTOKEN\n    example_shape: \"AUTHTOKEN <guid>\"\n  sources: [openapi/keyper-access-openapi.yml]\nnotes:\n- API keys / app secrets are obtained by registering a business account at app.keyper.io/business.\n- Invalid or expired credentials return\
  \ HTTP 401 with the keyper error envelope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyper/refs/heads/main/authentication/keyper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ticketing
- Access Control
- Events
- Developer Platform
- SDK
- Sports
- Arts and Culture
- Austria
---
