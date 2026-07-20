---
api_key_in: []
api_specs:
- filename: anything-openapi-original.json
  format: json
  label: Anything API
  slug: anything-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anything Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anything secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anything
provider_slug: anything
scheme_count: 1
schemes:
- description: 'Use your Anything API key as the Basic auth username and leave the password empty. Example credentials: anything_xxx:'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/anything-openapi-original.json
  type: http
slug: anything-authentication
source_filename: anything-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/anything-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Use your Anything API key as the Basic auth username and leave the password\n    empty. Example credentials: anything_xxx:'\n  sources:\n  - openapi/anything-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/authentication/anything-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- App Builder
- Low Code
- No Code
- Developer Tools
- AI Agents
- Mobile
---
