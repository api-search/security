---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Camtasia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Camtasia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Camtasia
provider_slug: camtasia
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token from TechSmith account authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/camtasia-asset-library-openapi.yml
  - openapi/camtasia-project-management-openapi.yml
  type: http
slug: camtasia-authentication
source_filename: camtasia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/camtasia-asset-library-openapi.yml, openapi/camtasia-project-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token from TechSmith account authentication\n  sources:\n  - openapi/camtasia-asset-library-openapi.yml\n  - openapi/camtasia-project-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/authentication/camtasia-authentication.yml
summary_line: http · 1 scheme
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
---
