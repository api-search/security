---
api_key_in: []
api_specs:
- filename: forto-openapi.yml
  format: yaml
  label: Forto Public API
  slug: forto-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forto/refs/heads/main/openapi/forto-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Forto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forto
provider_slug: forto
scheme_count: 1
schemes:
- description: Bearer token issued via the /tokens endpoint.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/forto-openapi.yml
  type: http
slug: forto-authentication
source_filename: forto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/forto-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: Bearer token issued via the /tokens endpoint.\n  sources:\n  - openapi/forto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forto/refs/heads/main/authentication/forto-authentication.yml
summary_line: http · 1 scheme
tags:
- Freight
- Logistics
- Supply Chain
- Shipping
- Freight Forwarding
- EDI
---
