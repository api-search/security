---
api_key_in:
- header
api_specs:
- filename: photoroom-account-api-openapi.yml
  format: yaml
  label: Photoroom Account API
  slug: photoroom-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/openapi/photoroom-account-api-openapi.yml
- filename: photoroom-edit-api-openapi.yml
  format: yaml
  label: Photoroom Edit API
  slug: photoroom-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/openapi/photoroom-edit-api-openapi.yml
- filename: photoroom-render-api-openapi.yml
  format: yaml
  label: Photoroom Render API
  slug: photoroom-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/openapi/photoroom-render-api-openapi.yml
- filename: photoroom-segment-api-openapi.yml
  format: yaml
  label: Photoroom Segment API
  slug: photoroom-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/openapi/photoroom-segment-api-openapi.yml
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
- Artificial Intelligence
- Image Editing
- Background Removal
- E-Commerce
- Visual
---
