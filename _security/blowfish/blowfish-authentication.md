---
api_key_in:
- header
api_specs:
- filename: blowfish-v20230308-openapi-original.yml
  format: yaml
  label: Blowfish Scan API
  slug: blowfish-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blowfish/refs/heads/main/openapi/blowfish-v20230308-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blowfish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blowfish secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blowfish
provider_slug: blowfish
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/blowfish-v20230308-openapi-original.yml
  type: apiKey
slug: blowfish-authentication
source_filename: blowfish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/blowfish-v20230308-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/blowfish-v20230308-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blowfish/refs/heads/main/authentication/blowfish-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Web3
- Blockchain
- Wallet
- Transaction Scanning
- Fraud Prevention
- Cryptocurrency
---
