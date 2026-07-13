---
api_key_in: []
api_specs:
- filename: amazon-app-studio-openapi.yaml
  format: yaml
  label: Amazon App Studio API
  slug: app-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-studio/refs/heads/main/openapi/amazon-app-studio-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon App Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon App Studio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon App Studio
provider_slug: amazon-app-studio
scheme_count: 1
schemes:
- bearerFormat: AWS Sig V4
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/amazon-app-studio-openapi.yaml
  type: http
slug: amazon-app-studio-authentication
source_filename: amazon-app-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-app-studio-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: AWS Sig V4\n  sources:\n  - openapi/amazon-app-studio-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-studio/refs/heads/main/authentication/amazon-app-studio-authentication.yml
summary_line: http · 1 scheme
tags:
- Generative AI
- Internal Tools
- Low-Code
- No-Code
---
