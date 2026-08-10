---
api_key_in:
- header
api_specs:
- filename: celsius-network-kyc-api-openapi.yml
  format: yaml
  label: Celsius Network KYC API
  slug: celsius-network-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/openapi/celsius-network-kyc-api-openapi.yml
- filename: celsius-network-users-api-openapi.yml
  format: yaml
  label: Celsius Network Users API
  slug: celsius-network-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/openapi/celsius-network-users-api-openapi.yml
- filename: celsius-network-utility-api-openapi.yml
  format: yaml
  label: Celsius Network Utility API
  slug: celsius-network-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/openapi/celsius-network-utility-api-openapi.yml
- filename: celsius-network-wallet-api-openapi.yml
  format: yaml
  label: Celsius Network Wallet API
  slug: celsius-network-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/openapi/celsius-network-wallet-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Celsius Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celsius Network secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Celsius Network
provider_slug: celsius-network
scheme_count: 3
schemes:
- description: Partner key issued by Celsius and securely provided to the partner. Required on every authenticated request, for every partnership type.
  in: header
  name: partnerToken
  parameter: X-Cel-Partner-Token
  sources:
  - openapi/celsius-network-partner-api-openapi.yml
  type: apiKey
- description: User token created by the partner for each of its users. Used by Segmented Integration partners.
  in: header
  name: userToken
  parameter: X-Cel-User-Token
  sources:
  - openapi/celsius-network-partner-api-openapi.yml
  type: apiKey
- description: API key issued by Celsius and securely provided to the partner. Used by Omnibus and Omnibus Treasury partners.
  in: header
  name: apiKey
  parameter: X-Cel-Api-Key
  sources:
  - openapi/celsius-network-partner-api-openapi.yml
  type: apiKey
slug: celsius-network-authentication
source_filename: celsius-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/celsius-network-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: partnerToken\n  type: apiKey\n  in: header\n  parameter: X-Cel-Partner-Token\n  description: Partner key issued by Celsius and securely provided to the partner. Required\n    on every authenticated request, for every partnership type.\n  sources:\n  - openapi/celsius-network-partner-api-openapi.yml\n- name: userToken\n  type: apiKey\n  in: header\n  parameter: X-Cel-User-Token\n  description: User token created by the partner for each of its users. Used by Segmented Integration\n    partners.\n  sources:\n  - openapi/celsius-network-partner-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Cel-Api-Key\n  description: API key issued by Celsius and securely provided to the partner. Used by Omnibus\n    and Omnibus Treasury partners.\n  sources:\n  - openapi/celsius-network-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/authentication/celsius-network-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Cryptocurrency
- Digital Assets
- Financial Services
- Lending
- Custody
- Wallet
- Interest
- KYC
- Retired
---
