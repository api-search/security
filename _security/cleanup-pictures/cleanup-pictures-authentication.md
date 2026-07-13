---
api_key_in:
- header
api_specs:
- filename: cleanup-pictures-openapi.yml
  format: yaml
  label: Cleanup.pictures Inpainting API
  slug: cleanup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanup-pictures/refs/heads/main/openapi/cleanup-pictures-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cleanup Pictures Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleanup.pictures secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cleanup.pictures
provider_slug: cleanup-pictures
scheme_count: 1
schemes:
- description: ClipDrop API key. Obtain via contact@clipdrop.co.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/cleanup-pictures-openapi.yml
  type: apiKey
slug: cleanup-pictures-authentication
source_filename: cleanup-pictures-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cleanup-pictures-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: ClipDrop API key. Obtain via contact@clipdrop.co.\n  sources:\n  - openapi/cleanup-pictures-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanup-pictures/refs/heads/main/authentication/cleanup-pictures-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Image Editing
- Object Removal
- Inpainting
- Visual
---
