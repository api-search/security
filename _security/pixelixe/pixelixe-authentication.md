---
api_key_in: []
api_specs:
- filename: pixelixe-authentication-api-openapi.yml
  format: yaml
  label: Pixelixe Authentication API
  slug: pixelixe-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelixe/refs/heads/main/openapi/pixelixe-authentication-api-openapi.yml
- filename: pixelixe-document-api-openapi.yml
  format: yaml
  label: Pixelixe Document API
  slug: pixelixe-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelixe/refs/heads/main/openapi/pixelixe-document-api-openapi.yml
- filename: pixelixe-graphic-api-openapi.yml
  format: yaml
  label: Pixelixe Graphic API
  slug: pixelixe-graphic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelixe/refs/heads/main/openapi/pixelixe-graphic-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pixelixe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixelixe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pixelixe
provider_slug: pixelixe
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pixelixe-openapi.yml
  type: http
slug: pixelixe-authentication
source_filename: pixelixe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pixelixe-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/pixelixe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelixe/refs/heads/main/authentication/pixelixe-authentication.yml
summary_line: http · 1 scheme
tags:
- Graphics
- Image
---
