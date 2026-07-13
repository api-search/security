---
api_key_in:
- query
api_specs:
- filename: imgbb-openapi.yml
  format: yaml
  label: ImgBB Image Upload API
  slug: image-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgbb/refs/heads/main/openapi/imgbb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Imgbb Authentication
name_suffix: Authentication
oauth_flows: []
overview: ImgBB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ImgBB
provider_slug: imgbb
scheme_count: 1
schemes:
- description: API key obtained from your ImgBB account settings at https://api.imgbb.com/. Pass as a query parameter named `key`.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/imgbb-openapi.yml
  type: apiKey
slug: imgbb-authentication
source_filename: imgbb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imgbb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key obtained from your ImgBB account settings at https://api.imgbb.com/.\n    Pass as a query parameter named `key`.\n  sources:\n  - openapi/imgbb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgbb/refs/heads/main/authentication/imgbb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Image Hosting
- Image Upload
- File Sharing
- Cloud Storage
- Media
- REST API
---
