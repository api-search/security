---
api_key_in:
- header
api_specs:
- filename: shopgo-management-openapi.yml
  format: yaml
  label: ShopGo Management API
  slug: shopgo-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-management-openapi.yml
- filename: shopgo-platform-openapi.yml
  format: yaml
  label: ShopGo Platform API
  slug: shopgo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shopgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShopGo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ShopGo
provider_slug: shopgo
scheme_count: 2
schemes:
- description: Dashboard user API key. Grants access to the tenant account the dashboard user belongs to. Obtained by POSTing email + password to /v1/management/auth/key.
  in: header
  name: UserApiKey
  obtain: POST https://api.shopgo.me/v1/management/auth/key
  parameter: X-API-KEY
  sources:
  - openapi/shopgo-management-openapi.yml
  - https://docs.shopgo.me/management-api/authentication/using-user-api-key.md
  test: GET https://api.shopgo.me/v1/management/auth/test
  type: apiKey
- companion_header: X-TENANT-ID
  description: Platform-level master API key. Can access any tenant account; intended for ShopGo internal use, provisioned via an approval process. Requires an additional X-TENANT-ID (or X-TENANT-NAME) header to select the target tenant.
  in: header
  name: PlatformApiKey
  parameter: X-API-KEY
  sources:
  - openapi/shopgo-platform-openapi.yml
  - https://docs.shopgo.me/management-api/authentication/using-platform-api-key.md
  test: GET https://api.shopgo.me/v1/platform/auth/test
  type: apiKey
slug: shopgo-authentication
source_filename: shopgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.shopgo.me/management-api/authentication.md\ndocs: https://docs.shopgo.me/management-api/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_headers: [X-API-KEY]\n  oauth2_flows: []\n  notes: >-\n    ShopGo uses API-key authentication only; there is no OAuth2/OIDC surface.\n    A permission model (see authorization) governs what an authenticated key can access.\nschemes:\n  - name: UserApiKey\n    type: apiKey\n    in: header\n    parameter: X-API-KEY\n    description: >-\n      Dashboard user API key. Grants access to the tenant account the dashboard\n      user belongs to. Obtained by POSTing email + password to\n      /v1/management/auth/key.\n    obtain: POST https://api.shopgo.me/v1/management/auth/key\n    test: GET https://api.shopgo.me/v1/management/auth/test\n    sources: [openapi/shopgo-management-openapi.yml, https://docs.shopgo.me/management-api/authentication/using-user-api-key.md]\n\
  \  - name: PlatformApiKey\n    type: apiKey\n    in: header\n    parameter: X-API-KEY\n    description: >-\n      Platform-level master API key. Can access any tenant account; intended for\n      ShopGo internal use, provisioned via an approval process. Requires an\n      additional X-TENANT-ID (or X-TENANT-NAME) header to select the target tenant.\n    companion_header: X-TENANT-ID\n    test: GET https://api.shopgo.me/v1/platform/auth/test\n    sources: [openapi/shopgo-platform-openapi.yml, https://docs.shopgo.me/management-api/authentication/using-platform-api-key.md]\npermissions:\n  model: per-key permission flags (dashboard + API)\n  docs: https://docs.shopgo.me/management-api/authorization\n  values:\n    - {name: home, relevance: dashboard-only}\n    - {name: orders, relevance: dashboard-and-api}\n    - {name: reports, relevance: dashboard-and-api}\n    - {name: products, relevance: dashboard-and-api}\n    - {name: customers, relevance: dashboard-and-api}\n    - {name: appearance,\
  \ relevance: dashboard-only}\n    - {name: settings, relevance: dashboard-and-api}\n  enforcement: >-\n    Missing permission returns 403 Forbidden; expired trial without subscription\n    returns 402 Payment Required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/authentication/shopgo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- eCommerce
- Online Stores
- Payments
- Shipping
- SaaS
- MENA
- Orders
---
