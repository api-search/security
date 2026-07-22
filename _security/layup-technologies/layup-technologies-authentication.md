---
api_key_in:
- header
api_specs:
- filename: layup-technologies-openapi-original.json
  format: json
  label: LayUp API
  slug: layup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layup-technologies/refs/heads/main/openapi/layup-technologies-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Layup Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: LayUp Technologies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LayUp Technologies
provider_slug: layup-technologies
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/layup-technologies-openapi-original.json
  type: apiKey
slug: layup-technologies-authentication
source_filename: layup-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/layup-technologies-openapi-original.json\ndocs: https://documentation.layup.co.za/#authentication\nnotes: >-\n  API-key based authentication. The key is passed in the apikey HTTP header on\n  every request. Separate sandbox and live keys; sandbox base URL\n  https://sandbox-api.layup.co.za, production https://api.layup.co.za. No OAuth\n  or OpenID Connect.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/layup-technologies-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layup-technologies/refs/heads/main/authentication/layup-technologies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Lay-By
- Save Now Buy Later
- BNPL
- Instalments
- Fintech
- South Africa
- DebiCheck
- E-commerce
- Merchants
---
