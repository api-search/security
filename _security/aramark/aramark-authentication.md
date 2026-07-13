---
api_key_in:
- header
api_specs:
- filename: marko-api.yml
  format: yaml
  label: Aramark Marko API
  slug: marko-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/marko-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aramark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aramark secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aramark
provider_slug: aramark
scheme_count: 1
schemes:
- description: API key for Marko platform authentication, obtained from the developer portal.
  in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/marko-api.yml
  type: apiKey
slug: aramark-authentication
source_filename: aramark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marko-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API key for Marko platform authentication, obtained from the developer portal.\n  sources:\n  - openapi/marko-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/authentication/aramark-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
---
