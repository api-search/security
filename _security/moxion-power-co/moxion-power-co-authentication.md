---
api_key_in: []
api_specs:
- filename: moxion-power-co-openapi.yml
  format: yaml
  label: Moxion Power Developer API
  slug: moxion-power-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxion-power-co/refs/heads/main/openapi/moxion-power-co-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Moxion Power Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moxion Power Co secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moxion Power Co
provider_slug: moxion-power-co
scheme_count: 1
schemes:
- description: 'An API key issued to a Service Account, sent in the Authorization header with a `bearer ` prefix, e.g. `Authorization: bearer <YOUR TOKEN HERE>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moxion-power-co-openapi.yml
  type: http
slug: moxion-power-co-authentication
source_filename: moxion-power-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.moxionpower.com/docs/authentication\ndocs: https://developer.moxionpower.com/docs/authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    An API key issued to a Service Account, sent in the Authorization header\n    with a `bearer ` prefix, e.g.\n    `Authorization: bearer <YOUR TOKEN HERE>`.\n  sources: [openapi/moxion-power-co-openapi.yml]\nnotes:\n- >-\n  Before an API key can be created, an identity in the form of a Service Account\n  must exist. Service Accounts are created by Account Admins in the API tab of\n  the Settings page.\n- >-\n  By default Service Accounts have no roles or permissions; these must currently\n  be set up manually by Moxion personnel. Permissions and the Account Admin role\n  are requested via an account manager or help@moxionpower.com.\nexample_request:\
  \ |-\n  curl 'http://api.moxionpower.com/developer/v1/organizations' \\\n    -H 'Authorization: bearer <YOUR TOKEN HERE>'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxion-power-co/refs/heads/main/authentication/moxion-power-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy Storage
- Mobile Power
- Battery
- Telemetry
- IoT
- Fleet Management
- Clean Energy
- Construction
- Device Metrics
---
