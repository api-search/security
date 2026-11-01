---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: insumermodel-com-agent-commerce-protocols-api-openapi.yml
  format: yaml
  label: insumermodel-com Agent Commerce Protocols API
  slug: insumermodel-com-agent-commerce-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-agent-commerce-protocols-api-openapi.yml
- filename: insumermodel-com-agent-onboarding-api-openapi.yml
  format: yaml
  label: insumermodel-com Agent Onboarding API
  slug: insumermodel-com-agent-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-agent-onboarding-api-openapi.yml
- filename: insumermodel-com-discounts-codes-api-openapi.yml
  format: yaml
  label: insumermodel-com Discounts & Codes API
  slug: insumermodel-com-discounts-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-discounts-codes-api-openapi.yml
- filename: insumermodel-com-discovery-api-openapi.yml
  format: yaml
  label: insumermodel-com Discovery API
  slug: insumermodel-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-discovery-api-openapi.yml
- filename: insumermodel-com-keys-billing-api-openapi.yml
  format: yaml
  label: insumermodel-com Keys & Billing API
  slug: insumermodel-com-keys-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-keys-billing-api-openapi.yml
- filename: insumermodel-com-merchant-setup-api-openapi.yml
  format: yaml
  label: insumermodel-com Merchant Setup API
  slug: insumermodel-com-merchant-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-merchant-setup-api-openapi.yml
- filename: insumermodel-com-platform-api-openapi.yml
  format: yaml
  label: insumermodel-com Platform API
  slug: insumermodel-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-platform-api-openapi.yml
- filename: insumermodel-com-point-of-sale-api-openapi.yml
  format: yaml
  label: insumermodel-com Point of Sale API
  slug: insumermodel-com-point-of-sale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-point-of-sale-api-openapi.yml
- filename: insumermodel-com-trust-fact-profiles-api-openapi.yml
  format: yaml
  label: insumermodel-com Trust Fact Profiles API
  slug: insumermodel-com-trust-fact-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-trust-fact-profiles-api-openapi.yml
- filename: insumermodel-com-wallet-auth-api-openapi.yml
  format: yaml
  label: insumermodel-com Wallet Auth API
  slug: insumermodel-com-wallet-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-wallet-auth-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Insumermodel Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: insumermodel-com secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: insumermodel-com
provider_slug: insumermodel-com
scheme_count: 2
schemes:
- description: 'API key in format: insr_live_ followed by 40 hex characters'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/insumermodel-com-openapi.json
  type: apiKey
- description: 'Wallet-signed authentication. Accepted on: POST /v1/attest, POST /v1/trust, POST /v1/trust/batch, GET /v1/credits, and POST /v1/credits/buy. Other endpoints return 501 for this scheme. Header value: `Wallet <base64(JSON({message, signature}))>` where `message` is a SIWE (EIP-4361) string with `Domain: api.insumermodel.com` and `signature` is an EIP-191 personal_sign over `message`. The signing wal'
  in: header
  name: WalletAuth
  parameter: Authorization
  sources:
  - openapi/insumermodel-com-openapi.json
  type: apiKey
slug: insumermodel-com-authentication
source_filename: insumermodel-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/insumermodel-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key in format: insr_live_ followed by 40 hex characters'\n  sources:\n  - openapi/insumermodel-com-openapi.json\n- name: WalletAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Wallet-signed authentication. Accepted on: POST /v1/attest, POST /v1/trust,\n    POST /v1/trust/batch, GET /v1/credits, and POST /v1/credits/buy. Other endpoints return\n    501 for this scheme. Header value: `Wallet <base64(JSON({message, signature}))>` where `message`\n    is a SIWE (EIP-4361) string with `Domain: api.insumermodel.com` and `signature` is an EIP-191\n    personal_sign over `message`. The signing wal'\n  sources:\n  - openapi/insumermodel-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/insumermodel-com/authentication/insumermodel-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Wallet Auth
- Blockchain
- AI Agents
- Condition-Based Access
- Crypto
- Developer Tools
---
