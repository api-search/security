---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FixedQR Authentication
name_suffix: Authentication
oauth_flows: []
overview: FixedQR secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FixedQR
provider_slug: fixedqr-com
scheme_count: 1
schemes:
- description: Optional. Paid API keys (coming soon).
  name: apiKey
  scheme: bearer
  sources:
  - openapi/fixedqr-com-openapi.json
  type: http
slug: fixedqr-com-authentication
source_filename: fixedqr-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fixedqr-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Optional. Paid API keys (coming soon).\n  sources:\n  - openapi/fixedqr-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fixedqr-com/authentication/fixedqr-com-authentication.yml
summary_line: http · 1 scheme
tags:
- QR
- Generator
- Free
- Privacy
---
