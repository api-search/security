---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hyperbolic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperbolic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hyperbolic
provider_slug: hyperbolic
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hyperbolic-openapi.yml
  type: http
slug: hyperbolic-authentication
source_filename: hyperbolic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperbolic-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/hyperbolic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbolic/refs/heads/main/authentication/hyperbolic-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- GPU
- Open Source
- Serverless
- Image Generation
- Audio
---
