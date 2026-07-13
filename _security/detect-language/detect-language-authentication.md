---
api_key_in: []
api_specs:
- filename: detect-language-openapi.yml
  format: yaml
  label: Detect Language
  slug: detect-language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/detect-language/refs/heads/main/openapi/detect-language-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Detect Language Authentication
name_suffix: Authentication
oauth_flows: []
overview: Detect Language secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Detect Language
provider_slug: detect-language
scheme_count: 1
schemes:
- description: Bearer token using the API key issued in the Detect Language dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/detect-language-openapi.yml
  type: http
slug: detect-language-authentication
source_filename: detect-language-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/detect-language-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token using the API key issued in the Detect Language dashboard.\n  sources:\n  - openapi/detect-language-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/detect-language/refs/heads/main/authentication/detect-language-authentication.yml
summary_line: http · 1 scheme
tags:
- Detection
- Languages
- Translation
---
