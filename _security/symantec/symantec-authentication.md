---
api_key_in: []
api_specs:
- filename: symantec-sepm-api-openapi.yml
  format: yaml
  label: Symantec Endpoint Protection Manager API
  slug: sepm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symantec/refs/heads/main/openapi/symantec-sepm-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Symantec Authentication
name_suffix: Authentication
oauth_flows: []
overview: Symantec secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Symantec
provider_slug: symantec
scheme_count: 1
schemes:
- description: Bearer token obtained from the /identity/authenticate endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/symantec-sepm-api-openapi.yml
  type: http
slug: symantec-authentication
source_filename: symantec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/symantec-sepm-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the /identity/authenticate endpoint\n  sources:\n  - openapi/symantec-sepm-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symantec/refs/heads/main/authentication/symantec-authentication.yml
summary_line: http · 1 scheme
tags:
- Broadcom
- Cybersecurity
- DLP
- EDR
- Endpoint Protection
- Endpoint Security
- Security
- Symantec
- Fortune 500
---
