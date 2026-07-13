---
api_key_in:
- header
api_specs:
- filename: flux-image-generation-openapi.yml
  format: yaml
  label: Flux Image Generation API
  slug: flux-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/openapi/flux-image-generation-openapi.yml
- filename: flux-image-editing-openapi.yml
  format: yaml
  label: Flux Image Editing API
  slug: flux-image-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/openapi/flux-image-editing-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flux Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flux secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flux
provider_slug: flux
scheme_count: 1
schemes:
- description: API key from the Black Forest Labs developer portal. Pass in the X-Key header for all authenticated requests.
  in: header
  name: apiKeyAuth
  parameter: X-Key
  sources:
  - openapi/flux-image-editing-openapi.yml
  - openapi/flux-image-generation-openapi.yml
  type: apiKey
slug: flux-authentication
source_filename: flux-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flux-image-editing-openapi.yml, openapi/flux-image-generation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Key\n  description: API key from the Black Forest Labs developer portal. Pass in the X-Key header\n    for all authenticated requests.\n  sources:\n  - openapi/flux-image-editing-openapi.yml\n  - openapi/flux-image-generation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/authentication/flux-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Image Generation
- Machine Learning
- Open Source
- Text to Image
---
