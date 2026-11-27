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
name: Noon Barbari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noon Barbari secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Noon Barbari
provider_slug: noonbarbari-xyz
scheme_count: 1
schemes:
- bearerFormat: nb_<env>_<token>
  description: 'Send ''Authorization: Bearer nb_live_…''. Create a key in your account.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/noonbarbari-xyz-openapi.json
  type: http
slug: noonbarbari-xyz-authentication
source_filename: noonbarbari-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/noonbarbari-xyz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: nb_<env>_<token>\n  description: 'Send ''Authorization: Bearer nb_live_…''. Create a key in your account.'\n  sources:\n  - openapi/noonbarbari-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/noonbarbari-xyz/authentication/noonbarbari-xyz-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Cryptocurrency
- Backtesting
- Trading
- Software-as-a-Service
---
