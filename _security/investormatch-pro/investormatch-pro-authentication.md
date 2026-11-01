---
anonymous_access: false
api_key_in: []
api_specs:
- filename: investormatch-pro-openapi.json
  format: json
  label: InvestorMatch.Pro API
  slug: investormatch-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/investormatch-pro/openapi/investormatch-pro-openapi.json
- filename: investormatch-pro-api-openapi.json
  format: json
  label: InvestorMatch.Pro API API
  slug: investormatch-pro-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/investormatch-pro/openapi/_original/investormatch-pro-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Investormatch Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: investormatch-pro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: investormatch-pro
provider_slug: investormatch-pro
scheme_count: 1
schemes:
- description: 'Pass your API key as a Bearer token: `Authorization: Bearer im_live_…` (production) or `Authorization: Bearer im_test_…` (test mode, no credits charged).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/investormatch-pro-openapi.json
  type: http
slug: investormatch-pro-authentication
source_filename: investormatch-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/investormatch-pro-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your API key as a Bearer token: `Authorization: Bearer im_live_…` (production)\n    or `Authorization: Bearer im_test_…` (test mode, no credits charged).'\n  sources:\n  - openapi/investormatch-pro-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/investormatch-pro/authentication/investormatch-pro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Fundraising
- VentureCapital
- Startup
---
