---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: xoomar-com-companies-api-openapi.yml
  format: yaml
  label: XOOMAR Companies API
  slug: xoomar-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-companies-api-openapi.yml
- filename: xoomar-com-crypto-api-openapi.yml
  format: yaml
  label: XOOMAR Crypto API
  slug: xoomar-com-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-crypto-api-openapi.yml
- filename: xoomar-com-macro-api-openapi.yml
  format: yaml
  label: XOOMAR Macro API
  slug: xoomar-com-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-macro-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Xoomar Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: XOOMAR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: XOOMAR
provider_slug: xoomar-com
scheme_count: 1
schemes:
- description: Free account key from /account
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/xoomar-com-openapi.json
  type: apiKey
slug: xoomar-com-authentication
source_filename: xoomar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/xoomar-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Free account key from /account\n  sources:\n  - openapi/xoomar-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/xoomar-com/authentication/xoomar-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Capital Markets
- Data
- Financial Services
- Software
---
