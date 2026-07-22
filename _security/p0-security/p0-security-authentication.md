---
api_key_in: []
api_specs:
- filename: p0-security-jit-openapi.yml
  format: yaml
  label: P0 Just-in-Time Access API
  slug: p0-security-jit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p0-security/refs/heads/main/openapi/p0-security-jit-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: P0 Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: P0 Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: P0 Security
provider_slug: p0-security
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/p0-security-jit-openapi.yml
  type: http
slug: p0-security-authentication
source_filename: p0-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/p0-security-jit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/p0-security-jit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p0-security/refs/heads/main/authentication/p0-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Privileged Access Management
- Identity and Access Management
- Just-in-Time Access
- Cloud Security
- Authorization
- Zero Trust
- Agentic Access
- MCP
---
