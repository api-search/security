---
api_key_in:
- header
api_specs:
- filename: checkly-openapi.json
  format: json
  label: Checkly
  slug: checkly
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Checkly
provider_slug: checkly
scheme_count: 2
schemes:
- description: API Key authentication for Checkly API. You can get your API key at https://app.checklyhq.com/settings/user/api-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/checkly-openapi.json
  type: http
- description: Your Checkly account ID. You can find it at https://app.checklyhq.com/settings/account/general
  in: header
  name: accountId
  parameter: X-Checkly-Account
  sources:
  - openapi/checkly-openapi.json
  type: apiKey
slug: checkly-authentication
source_filename: checkly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkly-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API Key authentication for Checkly API. You can get your API key at https://app.checklyhq.com/settings/user/api-keys\n  sources:\n  - openapi/checkly-openapi.json\n- name: accountId\n  type: apiKey\n  in: header\n  parameter: X-Checkly-Account\n  description: Your Checkly account ID. You can find it at https://app.checklyhq.com/settings/account/general\n  sources:\n  - openapi/checkly-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/authentication/checkly-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Monitoring
- Testing
---
