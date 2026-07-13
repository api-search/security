---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: OpenZeppelin Defender API
  slug: openzeppelin-defender-api
  spec_type: OpenAPI
  url: https://www.api-docs.defender.openzeppelin.com/
- filename: api
  format: yaml
  label: OpenZeppelin Relayer API
  slug: openzeppelin-relayer-api
  spec_type: OpenAPI
  url: https://docs.openzeppelin.com/relayer/1.4.x/api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openzeppelin Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenZeppelin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenZeppelin
provider_slug: openzeppelin
scheme_count: 1
schemes:
- name: bearer_auth
  scheme: bearer
  sources:
  - openapi/openzeppelin-relayer-openapi.json
  type: http
slug: openzeppelin-authentication
source_filename: openzeppelin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openzeppelin-relayer-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openzeppelin-relayer-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/authentication/openzeppelin-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- Smart Contracts
- Blockchain
- Security
- Ethereum
- DeFi
- Solidity
- Relayer
- Monitoring
- Auditing
---
