---
api_key_in: []
api_specs:
- filename: stanley-black-and-decker-tool-connect-api-openapi.yml
  format: yaml
  label: DEWALT Tool Connect API
  slug: dewalt-tool-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanley-black-and-decker/refs/heads/main/openapi/stanley-black-and-decker-tool-connect-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stanley Black And Decker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stanley Black & Decker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stanley Black & Decker
provider_slug: stanley-black-and-decker
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stanley-black-and-decker-tool-connect-api-openapi.yml
  type: http
slug: stanley-black-and-decker-authentication
source_filename: stanley-black-and-decker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stanley-black-and-decker-tool-connect-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/stanley-black-and-decker-tool-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanley-black-and-decker/refs/heads/main/authentication/stanley-black-and-decker-authentication.yml
summary_line: http · 1 scheme
tags:
- Tools
- Hardware
- Manufacturing
- IoT
- Connected Tools
- Fortune 500
---
