---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Class Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Class Technologies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Class Technologies
provider_slug: class-technologies
scheme_count: 1
schemes:
- description: API key secret issued from the Class admin portal (Edit API Key page). Scoped per key; see scopes/class-technologies-scopes.yml for the scope catalog.
  format: 'Authorization: Bearer [api_key_secret]'
  header: Authorization
  in: header
  name: apiKeyBearer
  scheme: bearer
  sources:
  - https://developer.class.com/
  type: http
slug: class-technologies-authentication
source_filename: class-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.class.com/\ndocs: https://developer.class.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\n  scope_model: true\n  notes: >-\n    Class uses scoped API-key secrets, presented as HTTP bearer tokens. Keys are\n    created in the Class admin portal and each key is granted a specific set of\n    scopes; a request that lacks a required scope returns 403 Forbidden.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer [api_key_secret]'\n  description: >-\n    API key secret issued from the Class admin portal (Edit API Key page). Scoped\n    per key; see scopes/class-technologies-scopes.yml for the scope catalog.\n  sources: [https://developer.class.com/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class-technologies/refs/heads/main/authentication/class-technologies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Edtech
- Education
- Virtual Classroom
- E-Learning
- LMS
- Online Learning
- Corporate Training
- Video Conferencing
---
