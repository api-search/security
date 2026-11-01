---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: fractal-is-approvalservice-api-openapi.yml
  format: yaml
  label: Fractal Approval Service API
  slug: fractal-is-approvalservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-approvalservice-api-openapi.yml
- filename: fractal-is-chainservice-api-openapi.yml
  format: yaml
  label: Fractal Chain Service API
  slug: fractal-is-chainservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-chainservice-api-openapi.yml
- filename: fractal-is-evmexperimentalservice-api-openapi.yml
  format: yaml
  label: Fractal EVM Experimental Service API
  slug: fractal-is-evmexperimentalservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-evmexperimentalservice-api-openapi.yml
- filename: fractal-is-fileservice-api-openapi.yml
  format: yaml
  label: Fractal File Service API
  slug: fractal-is-fileservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-fileservice-api-openapi.yml
- filename: fractal-is-inventorymanagementservice-api-openapi.yml
  format: yaml
  label: Fractal Inventory Management Service API
  slug: fractal-is-inventorymanagementservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-inventorymanagementservice-api-openapi.yml
- filename: fractal-is-linkaccountservice-api-openapi.yml
  format: yaml
  label: Fractal Link Account Service API
  slug: fractal-is-linkaccountservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-linkaccountservice-api-openapi.yml
- filename: fractal-is-marketplaceservice-api-openapi.yml
  format: yaml
  label: Fractal Marketplace Service API
  slug: fractal-is-marketplaceservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-marketplaceservice-api-openapi.yml
- filename: fractal-is-metagameservice-api-openapi.yml
  format: yaml
  label: Fractal Metagame Service API
  slug: fractal-is-metagameservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-metagameservice-api-openapi.yml
- filename: fractal-is-oauth-api-openapi.yml
  format: yaml
  label: Fractal OAuth API
  slug: fractal-is-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-oauth-api-openapi.yml
- filename: fractal-is-scoreservice-api-openapi.yml
  format: yaml
  label: Fractal Score Service API
  slug: fractal-is-scoreservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-scoreservice-api-openapi.yml
- filename: fractal-is-signinservicev2-api-openapi.yml
  format: yaml
  label: Fractal Sign In Service V2 API
  slug: fractal-is-signinservicev2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-signinservicev2-api-openapi.yml
- filename: fractal-is-solanaadminservice-api-openapi.yml
  format: yaml
  label: Fractal Solana Admin Service API
  slug: fractal-is-solanaadminservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-solanaadminservice-api-openapi.yml
- filename: fractal-is-solanamarketplaceservice-api-openapi.yml
  format: yaml
  label: Fractal Solana Marketplace Service API
  slug: fractal-is-solanamarketplaceservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-solanamarketplaceservice-api-openapi.yml
- filename: fractal-is-solanamintexperimentalservice-api-openapi.yml
  format: yaml
  label: Fractal Solana Mint Experimental Service API
  slug: fractal-is-solanamintexperimentalservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-solanamintexperimentalservice-api-openapi.yml
- filename: fractal-is-solanatransactionservice-api-openapi.yml
  format: yaml
  label: Fractal Solana Transaction Service API
  slug: fractal-is-solanatransactionservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-solanatransactionservice-api-openapi.yml
- filename: fractal-is-tournamentservice-api-openapi.yml
  format: yaml
  label: Fractal Tournament Service API
  slug: fractal-is-tournamentservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-tournamentservice-api-openapi.yml
- filename: fractal-is-transactionservice-api-openapi.yml
  format: yaml
  label: Fractal Transaction Service API
  slug: fractal-is-transactionservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-transactionservice-api-openapi.yml
- filename: fractal-is-walletservice-api-openapi.yml
  format: yaml
  label: Fractal Wallet Service API
  slug: fractal-is-walletservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-walletservice-api-openapi.yml
- filename: fractal-is-auth-service-api-openapi.yml
  format: yaml
  label: Fractal Auth Service API
  slug: fractal-is-auth-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractal-is/openapi/fractal-is-auth-service-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Fractal Is Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fractal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fractal
provider_slug: fractal-is
scheme_count: 2
schemes:
- description: 'Project API Token. Example: ''Authorization: Bearer <token>''

    see https://developers.fractal.is/server-auth'
  in: header
  name: projectApiToken
  parameter: Authorization
  sources:
  - openapi/fractal-is-api-openapi.yml
  - openapi/fractal-is-auth-api-openapi.yml
  type: apiKey
- name: sec0
  scheme: basic
  sources:
  - openapi/fractal-is-server-auth-api-openapi.yml
  type: http
slug: fractal-is-authentication
source_filename: fractal-is-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: derived\nsource: openapi/fractal-is-api-openapi.yml, openapi/fractal-is-auth-api-openapi.yml, openapi/fractal-is-server-auth-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: projectApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Project API Token. Example: 'Authorization: Bearer <token>'\n    see https://developers.fractal.is/server-auth\n  sources:\n  - openapi/fractal-is-api-openapi.yml\n  - openapi/fractal-is-auth-api-openapi.yml\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/fractal-is-server-auth-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fractal-is/authentication/fractal-is-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
---
