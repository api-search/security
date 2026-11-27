---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: counselor-guide-openapi.yml
  format: yaml
  label: Bicycle Guide Registry API
  slug: guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counselor-guide/openapi/counselor-guide-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Counselor Guide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Counselor Guide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Counselor Guide
provider_slug: counselor-guide
scheme_count: 1
schemes:
- description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid credentials ⇒ 401.'
  in: header
  name: bicycleGuideSecret
  parameter: x-bicycle-guide-secret
  sources:
  - openapi/counselor-guide-openapi.yml
  type: apiKey
slug: counselor-guide-authentication
source_filename: counselor-guide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/counselor-guide-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bicycleGuideSecret\n  type: apiKey\n  in: header\n  parameter: x-bicycle-guide-secret\n  description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret\n    header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid\n    credentials ⇒ 401.'\n  sources:\n  - openapi/counselor-guide-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/counselor-guide/authentication/counselor-guide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Counseling
- Psychotherapy
- Mental Health
- Education
- Professional Development
- Books
- MCP
---
