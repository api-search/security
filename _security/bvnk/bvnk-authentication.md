---
api_key_in:
- header
api_specs:
- filename: bvnk-address-api-openapi.yml
  format: yaml
  label: BVNK Address API
  slug: bvnk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-address-api-openapi.yml
- filename: bvnk-asset-pool-api-openapi.yml
  format: yaml
  label: BVNK Asset Pool API
  slug: bvnk-asset-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-asset-pool-api-openapi.yml
- filename: bvnk-channels-api-openapi.yml
  format: yaml
  label: BVNK Channels API
  slug: bvnk-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-channels-api-openapi.yml
- filename: bvnk-currencies-api-openapi.yml
  format: yaml
  label: BVNK Currencies API
  slug: bvnk-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-currencies-api-openapi.yml
- filename: bvnk-export-api-openapi.yml
  format: yaml
  label: BVNK Export API
  slug: bvnk-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-export-api-openapi.yml
- filename: bvnk-fee-api-openapi.yml
  format: yaml
  label: BVNK Fee API
  slug: bvnk-fee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-fee-api-openapi.yml
- filename: bvnk-key-pair-api-openapi.yml
  format: yaml
  label: BVNK Key Pair API
  slug: bvnk-key-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-key-pair-api-openapi.yml
- filename: bvnk-merchant-ids-api-openapi.yml
  format: yaml
  label: BVNK Merchant IDs API
  slug: bvnk-merchant-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-merchant-ids-api-openapi.yml
- filename: bvnk-network-api-openapi.yml
  format: yaml
  label: BVNK Network API
  slug: bvnk-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-network-api-openapi.yml
- filename: bvnk-payments-api-openapi.yml
  format: yaml
  label: BVNK Payments API
  slug: bvnk-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-payments-api-openapi.yml
- filename: bvnk-return-api-openapi.yml
  format: yaml
  label: BVNK Return API
  slug: bvnk-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-return-api-openapi.yml
- filename: bvnk-screening-api-openapi.yml
  format: yaml
  label: BVNK Screening API
  slug: bvnk-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-screening-api-openapi.yml
- filename: bvnk-trading-and-conversions-api-openapi.yml
  format: yaml
  label: BVNK Trading and Conversions API
  slug: bvnk-trading-and-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-trading-and-conversions-api-openapi.yml
- filename: bvnk-transaction-api-openapi.yml
  format: yaml
  label: BVNK Transaction API
  slug: bvnk-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-transaction-api-openapi.yml
- filename: bvnk-transaction-request-api-openapi.yml
  format: yaml
  label: BVNK Transaction Request API
  slug: bvnk-transaction-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-transaction-request-api-openapi.yml
- filename: bvnk-wallets-api-openapi.yml
  format: yaml
  label: BVNK Wallets API
  slug: bvnk-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-wallets-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Bvnk Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BVNK secures its APIs with apiKey, http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BVNK
provider_slug: bvnk
scheme_count: 4
schemes:
- description: 'Hawk Payload (see: https://github.com/hueniverse/hawk)'
  in: header
  name: Hawk
  parameter: Authorization
  sources:
  - openapi/bvnk-api-endpoints-openapi-original.yml
  type: apiKey
- name: openId
  openIdConnectUrl: https://auth.sandbox.layer1.com/auth/realms/bvnk/.well-known/openid-configuration
  sources:
  - openapi/bvnk-layer1-digital-asset-openapi-original.yml
  type: openIdConnect
- name: httpSignature
  scheme: signature
  sources:
  - openapi/bvnk-layer1-digital-asset-openapi-original.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.sandbox.layer1.com/auth/realms/bvnk/protocol/openid-connect/token
  name: oauth2
  sources:
  - openapi/bvnk-layer1-digital-asset-openapi-original.yml
  type: oauth2
slug: bvnk-authentication
source_filename: bvnk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: derived\nsource: openapi/bvnk-api-endpoints-openapi-original.yml, openapi/bvnk-layer1-digital-asset-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Hawk\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Hawk Payload (see: https://github.com/hueniverse/hawk)'\n  sources:\n  - openapi/bvnk-api-endpoints-openapi-original.yml\n- name: openId\n  type: openIdConnect\n  openIdConnectUrl: https://auth.sandbox.layer1.com/auth/realms/bvnk/.well-known/openid-configuration\n  sources:\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n- name: httpSignature\n  type: http\n  scheme: signature\n  sources:\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sandbox.layer1.com/auth/realms/bvnk/protocol/openid-connect/token\n\
  \    scopes: 0\n  sources:\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/authentication/bvnk-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Payments
- Stablecoins
- Cryptocurrency
- Wallets
- Virtual Accounts
- Cross-Border Payments
- Financial Services
- Cards
- Digital Assets
- Banking
- Compliance
---
