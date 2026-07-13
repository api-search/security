---
api_key_in:
- header
api_specs:
- filename: freepik-openapi.yml
  format: yaml
  label: Freepik
  slug: freepik
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freepik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freepik secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freepik
provider_slug: freepik
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: x-magnific-api-key
  sources:
  - openapi/freepik-openapi.yml
  type: apiKey
slug: freepik-authentication
source_filename: freepik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freepik-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-magnific-api-key\n  sources:\n  - openapi/freepik-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/authentication/freepik-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Graphics
- Illustrations
- Image Generation
- Photos
- Video Generation
---
