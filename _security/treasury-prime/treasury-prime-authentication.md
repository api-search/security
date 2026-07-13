---
api_key_in: []
api_specs:
- filename: treasury-prime-openapi.yml
  format: yaml
  label: Treasury Prime Bank API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Treasury Prime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Treasury Prime secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Treasury Prime
provider_slug: treasury-prime
scheme_count: 1
schemes:
- description: HTTP Basic Auth using API Key ID (username) and Secret (password).
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/treasury-prime-openapi.yml
  type: http
slug: treasury-prime-authentication
source_filename: treasury-prime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/treasury-prime-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using API Key ID (username) and Secret (password).\n  sources:\n  - openapi/treasury-prime-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/authentication/treasury-prime-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
---
