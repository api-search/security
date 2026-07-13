---
api_key_in:
- header
api_specs:
- filename: bot-butcher-openapi.yml
  format: yaml
  label: Bot Butcher Classification API
  slug: bot-butcher-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bot-butcher/refs/heads/main/openapi/bot-butcher-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bot Butcher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bot Butcher secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bot Butcher
provider_slug: bot-butcher
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/bot-butcher-openapi.yml
  type: apiKey
slug: bot-butcher-authentication
source_filename: bot-butcher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bot-butcher-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/bot-butcher-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bot-butcher/refs/heads/main/authentication/bot-butcher-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bots
- Spam Detection
- Contact Forms
- AI Classification
- Security
---
