---
api_key_in:
- header
api_specs:
- filename: justcall-openapi.yml
  format: yaml
  label: JustCall REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justcall/refs/heads/main/openapi/justcall-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Justcall Authentication
name_suffix: Authentication
oauth_flows: []
overview: JustCall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JustCall
provider_slug: justcall
scheme_count: 1
schemes:
- description: JustCall authentication. Pass the API key and API secret as defined in the JustCall Authentication documentation (typically combined and passed in the Authorization header).
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/justcall-openapi.yml
  type: apiKey
slug: justcall-authentication
source_filename: justcall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/justcall-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JustCall authentication. Pass the API key and API secret as defined in the JustCall\n    Authentication documentation (typically combined and passed in the Authorization header).\n  sources:\n  - openapi/justcall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justcall/refs/heads/main/authentication/justcall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Voice
- SMS
- Cloud Phone
- Contact Center
- Telephony
- Communications
---
