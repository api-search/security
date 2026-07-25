---
api_key_in: []
api_specs:
- filename: openzeppelin-health-api-openapi.yml
  format: yaml
  label: OpenZeppelin Health API
  slug: openzeppelin-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-health-api-openapi.yml
- filename: openzeppelin-metrics-api-openapi.yml
  format: yaml
  label: OpenZeppelin Metrics API
  slug: openzeppelin-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-metrics-api-openapi.yml
- filename: openzeppelin-networks-api-openapi.yml
  format: yaml
  label: OpenZeppelin Networks API
  slug: openzeppelin-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-networks-api-openapi.yml
- filename: openzeppelin-notifications-api-openapi.yml
  format: yaml
  label: OpenZeppelin Notifications API
  slug: openzeppelin-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-notifications-api-openapi.yml
- filename: openzeppelin-plugins-api-openapi.yml
  format: yaml
  label: OpenZeppelin Plugins API
  slug: openzeppelin-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-plugins-api-openapi.yml
- filename: openzeppelin-relayers-api-openapi.yml
  format: yaml
  label: OpenZeppelin Relayers API
  slug: openzeppelin-relayers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-relayers-api-openapi.yml
- filename: openzeppelin-signers-api-openapi.yml
  format: yaml
  label: OpenZeppelin Signers API
  slug: openzeppelin-signers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/openapi/openzeppelin-signers-api-openapi.yml
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
