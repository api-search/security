---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Dixa API
  slug: dixa-api
  spec_type: OpenAPI
  url: https://docs.dixa.io/openapi/dixa-api/beta/overview/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dixa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dixa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dixa
provider_slug: dixa
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/dixa-api.yaml
  type: apiKey
slug: dixa-authentication
source_filename: dixa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dixa-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/dixa-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/authentication/dixa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Customer Service
- Conversational
- Omnichannel
- CX
- Help Desk
- Chat
- Knowledge Base
---
