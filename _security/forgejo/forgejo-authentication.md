---
api_key_in:
- header
- query
api_specs:
- filename: swagger.v1.json
  format: json
  label: Forgejo REST API
  slug: forgejo-api
  spec_type: OpenAPI
  url: https://code.forgejo.org/swagger.v1.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Forgejo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forgejo secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Forgejo
provider_slug: forgejo
scheme_count: 5
schemes:
- description: API tokens must be prepended with "token" followed by a space.
  in: header
  name: AuthorizationHeaderToken
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/openapi.json
  type: http
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: header
  name: SudoHeader
  parameter: Sudo
  sources:
  - openapi/openapi.json
  type: apiKey
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: query
  name: SudoParam
  parameter: sudo
  sources:
  - openapi/openapi.json
  type: apiKey
- description: Must be used in combination with BasicAuth if two-factor authentication is enabled.
  in: header
  name: TOTPHeader
  parameter: X-FORGEJO-OTP
  sources:
  - openapi/openapi.json
  type: apiKey
slug: forgejo-authentication
source_filename: forgejo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: AuthorizationHeaderToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API tokens must be prepended with \"token\" followed by a space.\n  sources:\n  - openapi/openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/openapi.json\n- name: SudoHeader\n  type: apiKey\n  in: header\n  parameter: Sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/openapi.json\n- name: SudoParam\n  type: apiKey\n  in: query\n  parameter: sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/openapi.json\n- name: TOTPHeader\n  type: apiKey\n  in: header\n  parameter: X-FORGEJO-OTP\n  description: Must be used in combination\
  \ with BasicAuth if two-factor authentication is enabled.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/authentication/forgejo-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Git
- Source Code Management
- Self-Hosted
- DevOps
- CI/CD
- Open Source
- Forge
- Repositories
- Issues
- Pull Requests
---
