---
api_key_in:
- header
api_specs:
- filename: tavus-openapi.yml
  format: yaml
  label: Tavus API
  slug: tavus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tavus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tavus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tavus
provider_slug: tavus
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/tavus-openapi.yml
  type: apiKey
slug: tavus-authentication
source_filename: tavus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tavus-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/tavus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/authentication/tavus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Generative AI
- Video
- Conversational AI
- Avatars
- Replicas
- Personalization
- Real Time
- CVI
- Webhooks
---
