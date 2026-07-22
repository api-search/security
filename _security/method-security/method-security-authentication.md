---
api_key_in: []
api_specs:
- filename: method-security-openapi-original.yml
  format: yaml
  label: Method Platform API
  slug: method-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Method Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Method Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Method Security
provider_slug: method-security
scheme_count: 1
schemes:
- name: client-credentials
  scheme: bearer
  sources:
  - openapi/method-security-openapi-original.yml
  type: http
slug: method-security-authentication
source_filename: method-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/method-security-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: client-credentials\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/method-security-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/authentication/method-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Offensive Security
- Exposure Management
- Attack Surface Management
- Vulnerability Management
- Red Team
- AI Agents
- Government
---
