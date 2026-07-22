---
api_key_in:
- header
api_specs:
- filename: prewave-openapi-original.json
  format: json
  label: Public Prewave API
  slug: public-prewave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prewave/refs/heads/main/openapi/prewave-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prewave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prewave secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prewave
provider_slug: prewave
scheme_count: 1
schemes:
- description: Generate an API token at https://www.prewave.com/management/api and paste it in here.
  in: header
  name: Token authentication
  parameter: X-Auth-Token
  sources:
  - openapi/prewave-openapi-original.json
  type: apiKey
slug: prewave-authentication
source_filename: prewave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/prewave-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Token authentication\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Generate an API token at https://www.prewave.com/management/api and paste it\n    in here.\n  sources:\n  - openapi/prewave-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prewave/refs/heads/main/authentication/prewave-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Saas
- Supply Chain
- Risk Intelligence
- Sustainability
- Compliance
- EUDR
- Supplier Management
---
