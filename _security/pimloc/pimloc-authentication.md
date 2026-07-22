---
api_key_in: []
api_specs:
- filename: secureredact-openapi.yml
  format: yaml
  label: Secure Redact API
  slug: secure-redact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pimloc/refs/heads/main/openapi/secureredact-openapi.yml
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Pimloc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pimloc secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pimloc
provider_slug: pimloc
scheme_count: 2
schemes:
- credentials: client_id (username) + client_secret (password)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/secureredact-openapi.yml
  type: http
  used_on: /api/v3/token
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/secureredact-openapi.yml
  type: http
  used_on: all endpoints except /api/v3/token
slug: pimloc-authentication
source_filename: pimloc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.secureredact.co.uk\ndocs: https://docs.secureredact.co.uk\nsummary:\n  types: [http-basic, http-bearer]\n  model: token-exchange\n  description: >-\n    HTTP Basic authentication with a client_id / client_secret pair (generated\n    from the Secure Redact account page) is used only on the token endpoint to\n    obtain a short-lived JWT access token. That JWT bearer token authenticates\n    all other endpoints. Passing a username to the token endpoint yields a\n    user-scoped access token used for the Enterprise Flow.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    used_on: /api/v3/token\n    credentials: client_id (username) + client_secret (password)\n    sources: [openapi/secureredact-openapi.yml]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    used_on: all endpoints except /api/v3/token\n    sources: [openapi/secureredact-openapi.yml]\ntoken_endpoint:\
  \ https://app.secureredact.co.uk/api/v3/token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pimloc/refs/heads/main/authentication/pimloc-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Privacy
- Video Redaction
- Anonymization
- PII
- Data Protection
- Artificial Intelligence
- Compliance
- Video Analytics
---
