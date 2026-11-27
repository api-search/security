---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: clinicalleader-guide-openapi.yml
  format: yaml
  label: Bicycle Guide Registry API
  slug: guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clinicalleader-guide/openapi/clinicalleader-guide-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Clinical Leader Guide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clinical Leader Guide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clinical Leader Guide
provider_slug: clinicalleader-guide
scheme_count: 1
schemes:
- description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid credentials ⇒ 401.'
  in: header
  name: bicycleGuideSecret
  parameter: x-bicycle-guide-secret
  sources:
  - openapi/clinicalleader-guide-openapi.yml
  type: apiKey
slug: clinicalleader-guide-authentication
source_filename: clinicalleader-guide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/clinicalleader-guide-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bicycleGuideSecret\n  type: apiKey\n  in: header\n  parameter: x-bicycle-guide-secret\n  description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret\n    header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid\n    credentials ⇒ 401.'\n  sources:\n  - openapi/clinicalleader-guide-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/clinicalleader-guide/authentication/clinicalleader-guide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Clinical Leadership
- Patient Safety
- Healthcare
- Leadership
- Guides
- Publishing
- Education
---
