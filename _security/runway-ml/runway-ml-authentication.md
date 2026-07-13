---
api_key_in: []
api_specs:
- filename: runway-ml-openapi.yml
  format: yaml
  label: Runway API
  slug: runway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway-ml/refs/heads/main/openapi/runway-ml-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runway Ml Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runway
provider_slug: runway-ml
scheme_count: 1
schemes:
- description: Runway API key issued via the Runway Developer Portal, supplied as a bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runway-ml-openapi.yml
  type: http
slug: runway-ml-authentication
source_filename: runway-ml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runway-ml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Runway API key issued via the Runway Developer Portal, supplied as a bearer token\n    in the Authorization header.\n  sources:\n  - openapi/runway-ml-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway-ml/refs/heads/main/authentication/runway-ml-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Generative AI
- Video
- Image
- Text To Video
- Image To Video
- Text To Image
- Text To Speech
- Avatars
- Creative Tools
- Media
---
