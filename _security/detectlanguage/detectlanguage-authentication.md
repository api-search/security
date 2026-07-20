---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: DetectLanguage API
  slug: detectlanguage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/detectlanguage/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Detectlanguage Authentication
name_suffix: Authentication
oauth_flows: []
overview: DetectLanguage secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DetectLanguage
provider_slug: detectlanguage
scheme_count: 1
schemes:
- description: 'Pass your API key in the Authorization header as a Bearer token. Example: Authorization: Bearer [example key]'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: detectlanguage-authentication
source_filename: detectlanguage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your API key in the Authorization header as a Bearer token. Example: Authorization:\n    Bearer [example key]'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/detectlanguage/refs/heads/main/authentication/detectlanguage-authentication.yml
summary_line: http · 1 scheme
tags:
- Language Detection
- Natural Language Processing
- Text Analysis
- Machine Learning
- Multilingual
---
