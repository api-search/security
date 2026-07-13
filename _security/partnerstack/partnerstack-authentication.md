---
api_key_in: []
api_specs:
- filename: partnerstack-openapi.yml
  format: yaml
  label: PartnerStack
  slug: partnerstack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/partnerstack/refs/heads/main/openapi/partnerstack-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Partnerstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: PartnerStack secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PartnerStack
provider_slug: partnerstack
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/partnerstack-openapi.yml
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/partnerstack-openapi.yml
  type: http
slug: partnerstack-authentication
source_filename: partnerstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/partnerstack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/partnerstack-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/partnerstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partnerstack/refs/heads/main/authentication/partnerstack-authentication.yml
summary_line: http · 2 schemes
tags:
- Partnerships
- Affiliate
- SaaS
---
