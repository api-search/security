---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Twindo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Twindo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Twindo
provider_slug: twindo
scheme_count: 1
schemes:
- in: header
  name: TokenAuth
  scheme_hint: 'Authorization: Token <key> (Django REST Framework TokenAuthentication signaled by WWW-Authenticate: Token)'
  sources:
  - https://api.twindo.com/v1/
  type: apiKey
slug: twindo-authentication
source_filename: twindo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.twindo.com/v1/\nnotes: >-\n  Twindo does not publish public API authentication docs; API + SDK access is an\n  enterprise/partner offering (\"Integrations (SDK + API)\" per the company's LLM\n  JSON API profile). A live probe of the API host shows a Django REST\n  Framework-style API requiring token authentication.\nevidence:\n- url: https://api.twindo.com/v1/\n  status: 401\n  www_authenticate: Token\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  probed: '2026-07-21'\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  scheme_hint: 'Authorization: Token <key> (Django REST Framework TokenAuthentication signaled by WWW-Authenticate: Token)'\n  sources: [https://api.twindo.com/v1/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twindo/refs/heads/main/authentication/twindo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Spatial Intelligence
- LiDAR
- Scan to CAD
- BIM
- Digital Twins
- Reality Capture
- Architecture
- Construction
- Interior Design
---
