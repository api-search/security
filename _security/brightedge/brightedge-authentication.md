---
api_key_in:
- cookie
- header
api_specs:
- filename: brightedge-platform-openapi-original.json
  format: json
  label: BrightEdge Platform API
  slug: brightedge-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-platform-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Brightedge Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrightEdge secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BrightEdge
provider_slug: brightedge
scheme_count: 6
schemes:
- name: http_basic
  scheme: basic
  sources:
  - openapi/brightedge-platform-openapi-original.json
  type: http
- in: header
  name: forwarded_http_basic
  parameter: X-Forwarded-Authorization
  sources:
  - openapi/brightedge-platform-openapi-original.json
  type: apiKey
- in: cookie
  name: session_cookie
  parameter: BRIGHTEDGE
  sources:
  - openapi/brightedge-platform-openapi-original.json
  type: apiKey
- in: header
  name: session_header
  parameter: X-BRIGHTEDGE-SESSION
  sources:
  - openapi/brightedge-platform-openapi-original.json
  type: apiKey
- in: header
  name: api_token_header
  parameter: X-Token
  sources:
  - openapi/brightedge-platform-openapi-original.json
  type: apiKey
- in: header
  name: bearer_token
  parameter: Bearer-Token
  sources:
  - openapi/brightedge-platform-openapi-original.json
  type: apiKey
slug: brightedge-authentication
source_filename: brightedge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brightedge-platform-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: http_basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/brightedge-platform-openapi-original.json\n- name: forwarded_http_basic\n  type: apiKey\n  in: header\n  parameter: X-Forwarded-Authorization\n  sources:\n  - openapi/brightedge-platform-openapi-original.json\n- name: session_cookie\n  type: apiKey\n  in: cookie\n  parameter: BRIGHTEDGE\n  sources:\n  - openapi/brightedge-platform-openapi-original.json\n- name: session_header\n  type: apiKey\n  in: header\n  parameter: X-BRIGHTEDGE-SESSION\n  sources:\n  - openapi/brightedge-platform-openapi-original.json\n- name: api_token_header\n  type: apiKey\n  in: header\n  parameter: X-Token\n  sources:\n  - openapi/brightedge-platform-openapi-original.json\n- name: bearer_token\n  type: apiKey\n  in: header\n  parameter:\
  \ Bearer-Token\n  sources:\n  - openapi/brightedge-platform-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/authentication/brightedge-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Company
- SEO
- Search
- Content
- Marketing
- Analytics
- Keywords
- Enterprise
- AI Search
---
