---
api_key_in:
- header
api_specs:
- filename: hilos-openapi-original.yml
  format: yaml
  label: Hilos API
  slug: hilos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hilos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hilos secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hilos
provider_slug: hilos
scheme_count: 1
schemes:
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/hilos-openapi-original.yml
  type: apiKey
slug: hilos-authentication
source_filename: hilos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hilos-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/hilos-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/authentication/hilos-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- WhatsApp
- Messaging
- Automation
- CRM
- Conversational Commerce
- Chatbots
- Customer Engagement
- Marketing
---
