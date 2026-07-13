---
api_key_in: []
api_specs:
- filename: luma-labs-openapi.yml
  format: yaml
  label: Luma Dream Machine API
  slug: dream-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-labs/refs/heads/main/openapi/luma-labs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Luma Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luma AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Luma AI
provider_slug: luma-labs
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/luma-labs-openapi.yml
  type: http
slug: luma-labs-authentication
source_filename: luma-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/luma-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/luma-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma-labs/refs/heads/main/authentication/luma-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Generative AI
- Video
- Image
- Text To Video
- Image To Video
- Upscaling
- Reframing
- Dream Machine
- Ray
- Photon
- Creative Tools
---
