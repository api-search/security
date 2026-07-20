---
api_key_in: []
api_specs:
- filename: adaptive-security-openapi.json
  format: json
  label: Adaptive API
  slug: adaptive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/openapi/adaptive-security-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adaptive Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adaptive Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adaptive Security
provider_slug: adaptive-security
scheme_count: 1
schemes:
- description: 'API authentication token obtained from the Adaptive Admin portal (Settings → API Tokens). Include the token in the Authorization header as: Bearer [example key]'
  name: bearer-token
  scheme: bearer
  sources:
  - openapi/adaptive-security-openapi.json
  type: http
slug: adaptive-security-authentication
source_filename: adaptive-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/adaptive-security-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer-token\n  type: http\n  scheme: bearer\n  description: 'API authentication token obtained from the Adaptive Admin portal (Settings →\n    API Tokens). Include the token in the Authorization header as: Bearer [example key]'\n  sources:\n  - openapi/adaptive-security-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/authentication/adaptive-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Security Awareness Training
- Phishing Simulation
- Deepfake Defense
- AI Governance
- Social Engineering
- Reporting
- Compliance
---
