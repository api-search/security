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
name: GustoQR Authentication
name_suffix: Authentication
oauth_flows: []
overview: GustoQR secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GustoQR
provider_slug: gustoqr-com
scheme_count: 1
schemes:
- description: An API key from gustoqr.com/docs/api (sk-…), or its read-only form (gq_ro_…)
  name: apiKey
  scheme: bearer
  sources:
  - openapi/gustoqr-com-openapi.yml
  type: http
slug: gustoqr-com-authentication
source_filename: gustoqr-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/gustoqr-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: An API key from gustoqr.com/docs/api (sk-…), or its read-only form (gq_ro_…)\n  sources:\n  - openapi/gustoqr-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gustoqr-com/authentication/gustoqr-com-authentication.yml
summary_line: http · 1 scheme
tags:
- QR
- DigitalMenu
- RestaurantTech
- Artificial Intelligence
- Multilingual
---
