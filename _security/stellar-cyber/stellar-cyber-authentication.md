---
api_key_in: []
api_specs:
- filename: stellar-cyber-openapi.yml
  format: yaml
  label: Stellar Cyber Open XDR API
  slug: stellar-cyber
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stellar Cyber Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stellar Cyber secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stellar Cyber
provider_slug: stellar-cyber
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained from /access_token endpoint. Tokens expire after 10 minutes. API keys can also be used as Bearer tokens for the /access_token call.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stellar-cyber-openapi.yml
  type: http
slug: stellar-cyber-authentication
source_filename: stellar-cyber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stellar-cyber-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from /access_token endpoint. Tokens expire after 10 minutes.\n    API keys can also be used as Bearer tokens for the /access_token call.\n  sources:\n  - openapi/stellar-cyber-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/authentication/stellar-cyber-authentication.yml
summary_line: http · 1 scheme
tags:
- Cybersecurity
- Security
- XDR
- SIEM
- SOAR
- AI
---
