---
api_key_in:
- header
api_specs:
- filename: casap-openapi.json
  format: json
  label: Casap API
  slug: casap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casap/refs/heads/main/openapi/casap-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Casap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Casap secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Casap
provider_slug: casap
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/casap-openapi.json
  type: apiKey
- in: header
  name: user_uuid
  parameter: x-user-uuid
  sources:
  - openapi/casap-openapi.json
  type: apiKey
slug: casap-authentication
source_filename: casap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/casap-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/casap-openapi.json\n- name: user_uuid\n  type: apiKey\n  in: header\n  parameter: x-user-uuid\n  sources:\n  - openapi/casap-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casap/refs/heads/main/authentication/casap-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Fintech
- Disputes
- Chargebacks
- Fraud
- Payments
- Banking
- Dispute Resolution
- Agentic AI
---
