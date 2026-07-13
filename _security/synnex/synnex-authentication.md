---
api_key_in: []
api_specs:
- filename: synnex-streamone-ion-openapi.yml
  format: yaml
  label: TD SYNNEX StreamOne ION API
  slug: streamone-ion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synnex/refs/heads/main/openapi/synnex-streamone-ion-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synnex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synnex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synnex
provider_slug: synnex
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synnex-streamone-ion-openapi.yml
  type: http
slug: synnex-authentication
source_filename: synnex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synnex-streamone-ion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token\n  sources:\n  - openapi/synnex-streamone-ion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synnex/refs/heads/main/authentication/synnex-authentication.yml
summary_line: http · 1 scheme
tags:
- Technology Distribution
- IT Distribution
- Cloud Marketplace
- Fortune 100
- Supply Chain
---
