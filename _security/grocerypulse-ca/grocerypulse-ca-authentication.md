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
name: GroceryPulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: GroceryPulse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GroceryPulse
provider_slug: grocerypulse-ca
scheme_count: 1
schemes:
- description: Issued per subscriber as gp_live…
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/grocerypulse-ca-openapi.json
  type: http
slug: grocerypulse-ca-authentication
source_filename: grocerypulse-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/grocerypulse-ca-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Issued per subscriber as gp_live…\n  sources:\n  - openapi/grocerypulse-ca-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/grocerypulse-ca/authentication/grocerypulse-ca-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Grocery
- Price Data
- Canada
- Retail
---
