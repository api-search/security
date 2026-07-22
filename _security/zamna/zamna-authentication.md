---
api_key_in: []
api_specs:
- filename: zamna-paxcheck-openapi-original.json
  format: json
  label: Zamna Ready To Fly (PaxCheck) API
  slug: zamna-ready-to-fly-paxcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zamna/refs/heads/main/openapi/zamna-paxcheck-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zamna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zamna secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zamna
provider_slug: zamna
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/zamna-paxcheck-openapi-original.json
  type: http
slug: zamna-authentication
source_filename: zamna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zamna-paxcheck-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zamna-paxcheck-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zamna/refs/heads/main/authentication/zamna-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Aviation
- Travel
- Identity Verification
- Digital Identity
- Passenger Processing
- Airlines
- Border Security
- Document Verification
- KYC
---
