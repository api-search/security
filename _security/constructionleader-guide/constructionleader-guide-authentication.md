---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: constructionleader-guide-openapi.yml
  format: yaml
  label: Guide Registry API
  slug: guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/constructionleader-guide/openapi/constructionleader-guide-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Construction Leader Guide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Construction Leader Guide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Construction Leader Guide
provider_slug: constructionleader-guide
scheme_count: 1
schemes:
- description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid credentials ⇒ 401.'
  in: header
  name: bicycleGuideSecret
  parameter: x-bicycle-guide-secret
  sources:
  - openapi/constructionleader-guide-openapi.yml
  type: apiKey
slug: constructionleader-guide-authentication
source_filename: constructionleader-guide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/constructionleader-guide-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bicycleGuideSecret\n  type: apiKey\n  in: header\n  parameter: x-bicycle-guide-secret\n  description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret\n    header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid\n    credentials ⇒ 401.'\n  sources:\n  - openapi/constructionleader-guide-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/constructionleader-guide/authentication/constructionleader-guide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Construction
- Leadership
- Safety
- Guides
- Bicycle
---
