---
api_key_in:
- header
api_specs:
- filename: wideo-automation-openapi.yml
  format: yaml
  label: Wideo Video Automation API
  slug: wideo-video-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/openapi/wideo-automation-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wideo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wideo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wideo
provider_slug: wideo
scheme_count: 1
schemes:
- description: API key in UUID form, scoped to a specific account and permission set. Generated assets are isolated by account.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/wideo-automation-openapi.yml
  type: apiKey
slug: wideo-authentication
source_filename: wideo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wideo-automation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key in UUID form, scoped to a specific account and permission set. Generated\n    assets are isolated by account.\n  sources:\n  - openapi/wideo-automation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/authentication/wideo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Video
- Video Automation
- Content Creation
- Media
- Marketing
- Templates
- No-Code
---
