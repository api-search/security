---
api_key_in:
- header
api_specs:
- filename: influitive-events-openapi.json
  format: json
  label: Influitive Events API
  slug: influitive-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influitive/refs/heads/main/openapi/influitive-events-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Influitive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Influitive secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Influitive
provider_slug: influitive
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: Auhtorization Token
  sources:
  - openapi/influitive-events-openapi.json
  type: apiKey
- in: header
  name: sec1
  parameter: X_ORG_ID
  sources:
  - openapi/influitive-events-openapi.json
  type: apiKey
slug: influitive-authentication
source_filename: influitive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/influitive-events-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Auhtorization Token\n  sources:\n  - openapi/influitive-events-openapi.json\n- name: sec1\n  type: apiKey\n  in: header\n  parameter: X_ORG_ID\n  sources:\n  - openapi/influitive-events-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influitive/refs/heads/main/authentication/influitive-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Customer Advocacy
- Customer Community
- Customer Engagement
- Advocacy Marketing
- Referral Marketing
- Customer Loyalty
- Gamification
- Webhooks
- SaaS
---
