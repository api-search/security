---
api_key_in: []
api_specs:
- filename: spec.yaml
  format: yaml
  label: Zamzar File Conversion API
  slug: zamzar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/zamzar/zamzar-spec/main/openapi/spec.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zamzar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zamzar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zamzar
provider_slug: zamzar
scheme_count: 1
schemes:
- name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/zamzar-openapi.yaml
  type: http
slug: zamzar-authentication
source_filename: zamzar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zamzar-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zamzar-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zamzar/refs/heads/main/authentication/zamzar-authentication.yml
summary_line: http · 1 scheme
tags:
- File Conversion
- Documents
- Video
- Audio
- Images
- CAD
- REST API
---
