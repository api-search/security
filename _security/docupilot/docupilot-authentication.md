---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi-accounts.yaml
  format: yaml
  label: Docupilot API
  slug: docupilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupilot/refs/heads/main/openapi/openapi-accounts.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docupilot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Docupilot secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Docupilot
provider_slug: docupilot
scheme_count: 3
schemes:
- description: OAuth2 Bearer Token Authentication
  name: OAuthAuthentication
  scheme: bearer
  sources:
  - openapi/openapi-accounts.yaml
  - openapi/openapi-app.yaml
  type: http
- description: browser based login takes care of this
  in: cookie
  name: SessionAuthentication
  parameter: sessionid
  sources:
  - openapi/openapi-accounts.yaml
  - openapi/openapi-app.yaml
  type: apiKey
- description: Token-based authentication with required prefix "Basic"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/openapi-app.yaml
  type: apiKey
slug: docupilot-authentication
source_filename: docupilot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-accounts.yaml, openapi/openapi-app.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: OAuthAuthentication\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer Token Authentication\n  sources:\n  - openapi/openapi-accounts.yaml\n  - openapi/openapi-app.yaml\n- name: SessionAuthentication\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  description: browser based login takes care of this\n  sources:\n  - openapi/openapi-accounts.yaml\n  - openapi/openapi-app.yaml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Basic\"\n  sources:\n  - openapi/openapi-app.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docupilot/refs/heads/main/authentication/docupilot-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Document Generation
- PDF Generation
- Document Automation
- Template Engine
- eSignature
- Workflow Automation
---
