---
api_key_in:
- header
api_specs:
- filename: tickitto-openapi-original.json
  format: json
  label: Tickitto API
  slug: tickitto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tickitto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tickitto secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tickitto
provider_slug: tickitto
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: key
  sources:
  - openapi/tickitto-openapi-original.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/tickitto-openapi-original.json
  type: http
slug: tickitto-authentication
source_filename: tickitto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tickitto-openapi-original.json\ndocs: https://docs.tickitto.com/key-principles/authentication\nnotes: >-\n  Authenticate by sending your API key in the `key` request header (no password). All endpoints\n  require authentication and HTTPS; unauthenticated or plain-HTTP requests fail. Keys are issued\n  by a Tickitto account manager and are tied to your account settings (booking fees, search\n  restrictions). An HTTP bearer scheme is also defined in the spec.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: key\n  sources:\n  - openapi/tickitto-openapi-original.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tickitto-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/authentication/tickitto-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ticketing
- Events
- Marketplace
- Travel & Experiences
- Entertainment
- Payments
- Commerce
---
