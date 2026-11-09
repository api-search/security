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
name: Customs Dog Authentication
name_suffix: Authentication
oauth_flows: []
overview: customs.dog secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: customs.dog
provider_slug: customs-dog
scheme_count: 1
schemes:
- description: 'Per-household API key. Mint it in the web app: Settings → API keys.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/customs-dog-openapi.json
  type: http
slug: customs-dog-authentication
source_filename: customs-dog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/customs-dog-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Per-household API key. Mint it in the web app: Settings → API keys.'\n  sources:\n  - openapi/customs-dog-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/customs-dog/authentication/customs-dog-authentication.yml
summary_line: http · 1 scheme
tags:
- Pet travel
- Border crossing
- Customs
- Travel app
---
