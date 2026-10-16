---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: viberate-openapi-generated.yml
  format: yaml
  label: Viberate API
  slug: viberate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viberate/refs/heads/main/openapi/_ae-authored/viberate-openapi-generated.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Viberate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Viberate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Viberate
provider_slug: viberate
scheme_count: 1
schemes:
- description: API key to authorize requests.
  in: header
  name: Access-Key
  parameter: Access-Key
  sources:
  - openapi/viberate-openapi.json
  type: apiKey
slug: viberate-authentication
source_filename: viberate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/viberate-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Access-Key\n  type: apiKey\n  in: header\n  parameter: Access-Key\n  description: API key to authorize requests.\n  sources:\n  - openapi/viberate-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viberate/refs/heads/main/authentication/viberate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Music
- Analytics
- Data
- API
- Platform
---
