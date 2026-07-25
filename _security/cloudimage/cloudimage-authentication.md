---
api_key_in:
- header
api_specs:
- filename: cloudimage-filerobot-dam-api-openapi.yml
  format: yaml
  label: Cloudimage Filerobot DAM API
  slug: cloudimage-filerobot-dam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-filerobot-dam-api-openapi.yml
- filename: cloudimage-image-api-openapi.yml
  format: yaml
  label: Cloudimage Image API
  slug: cloudimage-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-image-api-openapi.yml
- filename: cloudimage-video-api-openapi.yml
  format: yaml
  label: Cloudimage Video API
  slug: cloudimage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-video-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudimage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudimage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudimage
provider_slug: cloudimage
scheme_count: 1
schemes:
- description: Filerobot DAM API key.
  in: header
  name: filerobotKey
  parameter: X-Filerobot-Key
  sources:
  - openapi/cloudimage-openapi.yml
  type: apiKey
slug: cloudimage-authentication
source_filename: cloudimage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudimage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: filerobotKey\n  type: apiKey\n  in: header\n  parameter: X-Filerobot-Key\n  description: Filerobot DAM API key.\n  sources:\n  - openapi/cloudimage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/authentication/cloudimage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Image Optimization
- Image CDN
- Resizing
- Transformation
- DAM
---
