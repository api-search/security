---
api_key_in: []
api_specs:
- filename: imgix-openapi.yml
  format: yaml
  label: Imgix Rendering API
  slug: imgix-rendering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgix/refs/heads/main/openapi/imgix-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Imgix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imgix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Imgix
provider_slug: imgix
scheme_count: 1
schemes:
- description: Bearer API key from the imgix dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/imgix-openapi.yml
  type: http
slug: imgix-authentication
source_filename: imgix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imgix-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API key from the imgix dashboard.\n  sources:\n  - openapi/imgix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgix/refs/heads/main/authentication/imgix-authentication.yml
summary_line: http · 1 scheme
tags:
- CDN
- Image Optimization
- Image Processing
- Media
---
