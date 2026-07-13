---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Temenos Transact Core Banking API
  slug: temenos-transact-core-banking-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/transact/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Temenos Transact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Temenos Transact secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Temenos Transact
provider_slug: temenos-transact
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token authentication. Obtain a token from the Temenos authentication endpoint using client credentials or authorization code flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/temenos-transact-core-banking-openapi.yml
  type: http
slug: temenos-transact-authentication
source_filename: temenos-transact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temenos-transact-core-banking-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token authentication. Obtain a token from the Temenos authentication\n    endpoint using client credentials or authorization code flow.\n  sources:\n  - openapi/temenos-transact-core-banking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/authentication/temenos-transact-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
---
