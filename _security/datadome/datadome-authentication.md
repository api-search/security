---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Datadome Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataDome secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataDome
provider_slug: datadome
scheme_count: 1
schemes:
- description: DataDome management API key issued in the customer dashboard.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/datadome-openapi.yml
  type: apiKey
slug: datadome-authentication
source_filename: datadome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datadome-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: DataDome management API key issued in the customer dashboard.\n  sources:\n  - openapi/datadome-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/authentication/datadome-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bot Mitigation
- Fraud Protection
- Account Protection
- Ad Fraud
- DDoS
- Real-Time
- Edge Security
- Application Security
- Agentic Trust
---
