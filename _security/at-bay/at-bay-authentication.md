---
api_key_in: []
api_specs:
- filename: at-bay-partner-api-openapi.yml
  format: yaml
  label: At-Bay Partner API
  slug: at-bay-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/openapi/at-bay-partner-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: At Bay Authentication
name_suffix: Authentication
oauth_flows: []
overview: At-Bay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: At-Bay
provider_slug: at-bay
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/at-bay-partner-api-openapi.yml
  type: http
slug: at-bay-authentication
source_filename: at-bay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/at-bay-partner-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/at-bay-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/authentication/at-bay-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Cyber Insurance
- InsurSec
- Insurtech
- Tech E&O
- Professional Liability
- MPL
- Managed Detection And Response
- MDR
- Security Monitoring
- Email Security
- Endpoint Security
- Incident Response
- Brokers
- Quoting
- Binding
- Policy Lifecycle
- Webhooks
---
