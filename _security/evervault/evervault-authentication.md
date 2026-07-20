---
api_key_in: []
api_specs:
- filename: evervault-openapi-original.json
  format: json
  label: Evervault API
  slug: evervault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Evervault Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evervault secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Evervault
provider_slug: evervault
scheme_count: 3
schemes:
- description: Authentication using an API key. The username is the App ID and the password is the API Key (base64 App-ID:API-Key).
  name: ApiKey
  scheme: basic
  sources:
  - openapi/evervault-openapi-original.json
  type: http
- bearerFormat: RunToken
  description: 'Authentication using a short-lived Function run token shareable with clients. Authorization header: "RunToken <Function Run Token>".'
  name: TokenAuth
  scheme: bearer
  sources:
  - openapi/evervault-openapi-original.json
  type: http
- bearerFormat: Token
  description: 'Authentication using a short-lived client-side token. Authorization header: "Token <Client-Side Token>".'
  name: ClientSideToken
  scheme: bearer
  sources:
  - openapi/evervault-openapi-original.json
  type: http
slug: evervault-authentication
source_filename: evervault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/evervault-openapi-original.json + https://docs.evervault.com/developers/api-keys\ndocs: https://docs.evervault.com/developers/api-keys\nsummary:\n  types:\n  - http\n  http_schemes: [basic, bearer]\n  note: API keys can be created, scoped, rotated, and revoked. Short-lived bearer tokens are minted for client-side and Function-run contexts.\nschemes:\n- name: ApiKey\n  type: http\n  scheme: basic\n  description: Authentication using an API key. The username is the App ID and the password is the API Key (base64 App-ID:API-Key).\n  sources:\n  - openapi/evervault-openapi-original.json\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: RunToken\n  description: 'Authentication using a short-lived Function run token shareable with clients. Authorization header: \"RunToken <Function Run Token>\".'\n  sources:\n  - openapi/evervault-openapi-original.json\n- name: ClientSideToken\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: Token\n  description: 'Authentication using a short-lived client-side token. Authorization header: \"Token <Client-Side Token>\".'\n  sources:\n  - openapi/evervault-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/authentication/evervault-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Data
- Security
- Encryption
- Payments
- PCI Compliance
- Tokenization
- Cards
- Developer Tools
---
