---
api_key_in: []
api_specs:
- filename: chime-partner-api-openapi.yml
  format: yaml
  label: Chime Partner API
  slug: chime-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chime/refs/heads/main/openapi/chime-partner-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chime secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chime
provider_slug: chime
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/chime-partner-api-openapi.yml
  type: http
slug: chime-authentication
source_filename: chime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chime-partner-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token\n  sources:\n  - openapi/chime-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chime/refs/heads/main/authentication/chime-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Neobank
- Banking
- Checking Accounts
- Savings Accounts
- Early Paycheck Access
- Credit Building
- Peer-to-Peer Payments
- Consumer Banking
---
