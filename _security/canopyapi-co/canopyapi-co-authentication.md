---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Canopyapi Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: canopyapi-co declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: canopyapi-co
provider_slug: canopyapi-co
scheme_count: 2
schemes:
- evidence: 'Both require an API-KEY header or Authorization: Bearer YOUR_API_KEY header'
  header: API-KEY
  location: header
  name: API-KEY
  type: apiKey
- evidence: 'Both require an API-KEY header or Authorization: Bearer YOUR_API_KEY header'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
slug: canopyapi-co-authentication
source_filename: canopyapi-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.canopyapi.co/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.canopyapi.co/\nsources:\n- https://docs.canopyapi.co/\nschemes:\n- type: apiKey\n  name: API-KEY\n  evidence: 'Both require an API-KEY header or Authorization: Bearer YOUR_API_KEY header'\n  location: header\n  header: API-KEY\n- type: http-bearer\n  name: Authorization\n  evidence: 'Both require an API-KEY header or Authorization: Bearer YOUR_API_KEY header'\n  location: header\n  header: Authorization\ndocs: https://docs.canopyapi.co/\n"
source_yaml_url: https://artifacts.apis.io/canopyapi-co/authentication/canopyapi-co-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Amazon
- Data
- API
- E-commerce
- Pricing
---
