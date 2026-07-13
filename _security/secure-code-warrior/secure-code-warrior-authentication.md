---
api_key_in:
- header
api_specs:
- filename: secure-code-warrior-portal-openapi.yml
  format: yaml
  label: Secure Code Warrior Portal API
  slug: secure-code-warrior-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secure-code-warrior/refs/heads/main/openapi/secure-code-warrior-portal-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Secure Code Warrior Authentication
name_suffix: Authentication
oauth_flows: []
overview: Secure Code Warrior secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Secure Code Warrior
provider_slug: secure-code-warrior
scheme_count: 1
schemes:
- description: Report API key, Admin API key, or Team API Key
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/secure-code-warrior-portal-openapi.yml
  type: apiKey
slug: secure-code-warrior-authentication
source_filename: secure-code-warrior-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/secure-code-warrior-portal-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Report API key, Admin API key, or Team API Key\n  sources:\n  - openapi/secure-code-warrior-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secure-code-warrior/refs/heads/main/authentication/secure-code-warrior-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Security
- Developer Training
- Security Education
- AppSec
- Secure Coding
- DevSecOps
---
