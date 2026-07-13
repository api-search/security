---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: ConvertAPI
  slug: convertapi
  spec_type: OpenAPI
  url: https://v2.convertapi.com/info/openapi
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Convertapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConvertAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ConvertAPI
provider_slug: convertapi
scheme_count: 1
schemes:
- description: '[Get `Secret`](https://www.convertapi.com/a/secret)'
  name: secret
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: convertapi-authentication
source_filename: convertapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: secret\n  type: http\n  scheme: bearer\n  description: '[Get `Secret`](https://www.convertapi.com/a/secret)'\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertapi/refs/heads/main/authentication/convertapi-authentication.yml
summary_line: http · 1 scheme
tags:
- File Conversion
- PDF
- Documents
- Images
- Audio
- Video
- E-books
- Office Documents
- Batch Processing
---
