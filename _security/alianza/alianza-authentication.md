---
api_key_in:
- header
api_specs:
- filename: alianza-openapi-original.yml
  format: yaml
  label: Alianza Public API
  slug: alianza-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/openapi/alianza-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Alianza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alianza secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alianza
provider_slug: alianza
scheme_count: 1
schemes:
- in: header
  name: X-Auth-Token
  parameter: X-AUTH-TOKEN
  sources:
  - openapi/alianza-openapi-original.yml
  type: apiKey
slug: alianza-authentication
source_filename: alianza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/alianza-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Auth-Token\n  type: apiKey\n  in: header\n  parameter: X-AUTH-TOKEN\n  sources:\n  - openapi/alianza-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/authentication/alianza-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Communications
- Cloud Communications
- Voice
- VoIP
- Telecommunications
- UCaaS
- SIP Trunking
- Telephone Numbers
- CPaaS
- Service Providers
---
