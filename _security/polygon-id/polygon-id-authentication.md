---
api_key_in: []
api_specs:
- filename: api.yaml
  format: yaml
  label: Polygon ID Issuer Node API
  slug: polygon-id-issuer-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/0xPolygonID/issuer-node/main/api/api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polygon Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polygon ID secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Polygon ID
provider_slug: polygon-id
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/issuer-node-api.yaml
  type: http
slug: polygon-id-authentication
source_filename: polygon-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/issuer-node-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/issuer-node-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/authentication/polygon-id-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Verifiable Credentials
- Zero-Knowledge Proofs
- Self-Sovereign Identity
- Decentralized Identity
- Blockchain
- Web3
- KYC
---
