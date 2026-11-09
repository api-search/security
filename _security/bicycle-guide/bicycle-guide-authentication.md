---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bicycle-guide-guide-registry-api-openapi.yml
  format: yaml
  label: Bicycle Guide Guide Registry API
  slug: bicycle-guide-guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bicycle-guide/openapi/bicycle-guide-guide-registry-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bicycle Guide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bicycle Guide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bicycle Guide
provider_slug: bicycle-guide
scheme_count: 1
schemes:
- description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid credentials ⇒ 401.'
  in: header
  name: bicycleGuideSecret
  parameter: x-bicycle-guide-secret
  sources:
  - openapi/bicycle-guide-openapi.json
  type: apiKey
slug: bicycle-guide-authentication
source_filename: bicycle-guide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bicycle-guide-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bicycleGuideSecret\n  type: apiKey\n  in: header\n  parameter: x-bicycle-guide-secret\n  description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret\n    header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid\n    credentials ⇒ 401.'\n  sources:\n  - openapi/bicycle-guide-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bicycle-guide/authentication/bicycle-guide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Guides
- Artificial Intelligence
- Education
- Library
---
