---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Temsor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Temsor secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Temsor
provider_slug: temsor-com
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/temsor-com-openapi.json
  type: http
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/temsor-com-openapi.json
  type: apiKey
slug: temsor-com-authentication
source_filename: temsor-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/temsor-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/temsor-com-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/temsor-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/temsor-com/authentication/temsor-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Voice
- Communications
- SaaS
- Telephony
---
