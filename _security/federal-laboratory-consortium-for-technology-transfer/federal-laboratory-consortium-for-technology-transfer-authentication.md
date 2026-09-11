---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml
  format: yaml
  label: FLC Greenbook API
  slug: flc-greenbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-laboratory-consortium-for-technology-transfer/refs/heads/main/openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Federal Laboratory Consortium For Technology Transfer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Laboratory Consortium for Technology Transfer secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Federal Laboratory Consortium for Technology Transfer
provider_slug: federal-laboratory-consortium-for-technology-transfer
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml
  type: http
- description: Mobile app key (for sync-sections, mobile-app-sections, search)
  in: header
  name: app-key
  parameter: app-key
  sources:
  - openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml
  type: apiKey
slug: federal-laboratory-consortium-for-technology-transfer-authentication
source_filename: federal-laboratory-consortium-for-technology-transfer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: derived\nsource: openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml\n- name: app-key\n  type: apiKey\n  in: header\n  parameter: app-key\n  description: Mobile app key (for sync-sections, mobile-app-sections, search)\n  sources:\n  - openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-laboratory-consortium-for-technology-transfer/refs/heads/main/authentication/federal-laboratory-consortium-for-technology-transfer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Federal-Government
- Technology-Transfer
- Research
- Laboratories
- Government
- Innovation
- Search
---
