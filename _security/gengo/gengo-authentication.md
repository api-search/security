---
api_key_in:
- query
api_specs:
- filename: gengo-openapi.yml
  format: yaml
  label: Gengo API
  slug: gengo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gengo/refs/heads/main/openapi/gengo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gengo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gengo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gengo
provider_slug: gengo
scheme_count: 1
schemes:
- description: Public API key identifying the account. Every authenticated call must also include `ts` (Unix epoch) and `api_sig` (HMAC-SHA1 of `ts` keyed by the account private key). Keys are created on the account API settings page.
  in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/gengo-openapi.yml
  type: apiKey
slug: gengo-authentication
source_filename: gengo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gengo-openapi.yml\ndocs: https://developers.gengo.com/v2/authentication/\nmodel: >-\n  Custom API-key signature. Every restricted call is signed: take the current Unix\n  epoch as `ts`, compute the HMAC-SHA1 of `ts` keyed by the account private_key, and\n  send that as `api_sig` alongside the public `api_key`. The public/private key pair\n  functions as username/password and is generated on the account API settings page.\n  A few Service endpoints (language_pairs, languages, unit_count) require only api_key.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  signature: hmac-sha1\n  signed_params: [api_key, api_sig, ts]\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Public API key identifying the account. Every authenticated call must also include\n    `ts` (Unix epoch) and `api_sig` (HMAC-SHA1 of `ts` keyed by the account private key). Keys\n    are created on\
  \ the account API settings page.\n  sources:\n  - openapi/gengo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gengo/refs/heads/main/authentication/gengo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Translation
- Localization
- Human Translation
- Language Services
- Internationalization
- Content
- Text
---
