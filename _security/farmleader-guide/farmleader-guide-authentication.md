---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: farmleader-guide-openapi.json
  format: json
  label: Farm Leader Guide API
  slug: farm-leader-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farmleader-guide/openapi/farmleader-guide-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Farm Leader Guide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farm Leader Guide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Farm Leader Guide
provider_slug: farmleader-guide
scheme_count: 1
schemes:
- description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid credentials ⇒ 401.'
  in: header
  name: bicycleGuideSecret
  parameter: x-bicycle-guide-secret
  sources:
  - openapi/farmleader-guide-openapi.json
  type: apiKey
slug: farmleader-guide-authentication
source_filename: farmleader-guide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/farmleader-guide-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bicycleGuideSecret\n  type: apiKey\n  in: header\n  parameter: x-bicycle-guide-secret\n  description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret\n    header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid\n    credentials ⇒ 401.'\n  sources:\n  - openapi/farmleader-guide-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/farmleader-guide/authentication/farmleader-guide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Agriculture
- Farming
- Guides
- Community
---
