---
api_key_in: []
api_specs:
- filename: cryptoquant-openapi.yml
  format: yaml
  label: CryptoQuant API
  slug: cryptoquant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/openapi/cryptoquant-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cryptoquant Authentication
name_suffix: Authentication
oauth_flows: []
overview: CryptoQuant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CryptoQuant
provider_slug: cryptoquant
scheme_count: 1
schemes:
- description: API key passed as bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cryptoquant-openapi.yml
  type: http
slug: cryptoquant-authentication
source_filename: cryptoquant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cryptoquant-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as bearer token in the Authorization header.\n  sources:\n  - openapi/cryptoquant-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/authentication/cryptoquant-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- On-Chain Analytics
- Market Data
- Derivatives
---
