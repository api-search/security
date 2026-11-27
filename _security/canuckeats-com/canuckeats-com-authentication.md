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
name: Canuck Eats Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canuck Eats secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Canuck Eats
provider_slug: canuckeats-com
scheme_count: 1
schemes:
- description: API key from POST /register
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/canuckeats-com-openapi.json
  type: http
slug: canuckeats-com-authentication
source_filename: canuckeats-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/canuckeats-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from POST /register\n  sources:\n  - openapi/canuckeats-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/canuckeats-com/authentication/canuckeats-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Food Delivery
- Canada
- Price Comparison
- Restaurant
- Marketplace
---
