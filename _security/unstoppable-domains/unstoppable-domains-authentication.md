---
api_key_in: []
api_specs:
- filename: unstoppable-domains-resolution-api-openapi.yaml
  format: yaml
  label: Unstoppable Domains Resolution API
  slug: unstoppable-domains-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-resolution-api-openapi.yaml
- filename: unstoppable-domains-partner-api-openapi.yaml
  format: yaml
  label: Unstoppable Domains Partner API
  slug: unstoppable-domains-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-partner-api-openapi.yaml
- filename: unstoppable-domains-reseller-api-openapi.yaml
  format: yaml
  label: Unstoppable Domains Reseller API
  slug: unstoppable-domains-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-reseller-api-openapi.yaml
- filename: unstoppable-domains-user-api-openapi.json
  format: json
  label: Unstoppable Domains User API
  slug: unstoppable-domains-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-user-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unstoppable Domains Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unstoppable Domains secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unstoppable Domains
provider_slug: unstoppable-domains
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/unstoppable-domains-partner-api-openapi.yaml
  - openapi/unstoppable-domains-reseller-api-openapi.yaml
  - openapi/unstoppable-domains-resolution-api-openapi.yaml
  - openapi/unstoppable-domains-user-api-openapi.json
  type: http
slug: unstoppable-domains-authentication
source_filename: unstoppable-domains-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unstoppable-domains-partner-api-openapi.yaml, openapi/unstoppable-domains-reseller-api-openapi.yaml,\n  openapi/unstoppable-domains-resolution-api-openapi.yaml, openapi/unstoppable-domains-user-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/unstoppable-domains-partner-api-openapi.yaml\n  - openapi/unstoppable-domains-reseller-api-openapi.yaml\n  - openapi/unstoppable-domains-resolution-api-openapi.yaml\n  - openapi/unstoppable-domains-user-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/authentication/unstoppable-domains-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- Blockchain
- Domain Names
- NFT Domains
- Crypto
- Resolution
- DNS
- Decentralized
- Ethereum
- Polygon
---
