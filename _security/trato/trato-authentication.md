---
api_key_in: []
api_specs:
- filename: trato-openapi.yml
  format: yaml
  label: TRATO Contract API
  slug: trato-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trato/refs/heads/main/openapi/trato-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Trato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trato secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trato
provider_slug: trato
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trato-openapi.yml
  - https://developer.trato.io/
  type: http
slug: trato-authentication
source_filename: trato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.trato.io/\ndocs: https://developer.trato.io/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    TRATO authenticates every API call with a JWT bearer token sent in the\n    Authorization header (`Authorization: Bearer {TOKEN}`). The token is\n    mandatory on every request. Developers obtain the token from their TRATO\n    profile security settings (Profile > Security). No OAuth2 authorization\n    flow or API-key parameter is documented — the JWT is issued from the\n    account profile.\ntoken_source: https://clm-test.trato.io/profile?menu=profile-security\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    header: Authorization\n    sources: [openapi/trato-openapi.yml, https://developer.trato.io/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trato/refs/heads/main/authentication/trato-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Contract Management
- Contract Lifecycle Management
- Electronic Signature
- Legaltech
- Document Management
- Workflow Automation
- Legal
---
