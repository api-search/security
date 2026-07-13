---
api_key_in:
- header
api_specs:
- filename: photoroom-openapi.yml
  format: yaml
  label: Photoroom API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/openapi/photoroom-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Photoroom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Photoroom secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Photoroom
provider_slug: photoroom
scheme_count: 1
schemes:
- description: Get you API Key [here](https://app.photoroom.com/api-dashboard)
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/photoroom-openapi.yml
  type: apiKey
slug: photoroom-authentication
source_filename: photoroom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/photoroom-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Get you API Key [here](https://app.photoroom.com/api-dashboard)\n  sources:\n  - openapi/photoroom-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/authentication/photoroom-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Image Editing
- Background Removal
- E-commerce
- Visual
---
