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
name: Coderifts Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeRifts secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CodeRifts
provider_slug: coderifts
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/coderifts-openapi.json
  type: apiKey
- name: bearer
  scheme: bearer
  sources:
  - openapi/coderifts-openapi.json
  type: http
slug: coderifts-authentication
source_filename: coderifts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: derived\nsource: openapi/coderifts-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/coderifts-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/coderifts-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coderifts/refs/heads/main/authentication/coderifts-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Verification
- Compliance
- Platform
---
