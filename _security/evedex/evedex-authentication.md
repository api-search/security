---
api_key_in:
- header
api_specs:
- filename: evedex-auth-openapi.json
  format: json
  label: Auth Service
  slug: auth-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-auth-openapi.json
- filename: evedex-exchange-openapi.json
  format: json
  label: Exchange Service
  slug: exchange-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-exchange-openapi.json
- filename: evedex-market-data-openapi.json
  format: json
  label: Market Data Service
  slug: market-data-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-market-data-openapi.json
- filename: evedex-referral-openapi.json
  format: json
  label: Referral / Affiliate Service
  slug: referral-affiliate-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-referral-openapi.json
- filename: evedex-notifications-openapi.json
  format: json
  label: Notifications Service
  slug: notifications-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-notifications-openapi.json
- filename: evedex-academy-openapi.json
  format: json
  label: Academy Service
  slug: academy-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-academy-openapi.json
- filename: evedex-game-openapi.json
  format: json
  label: Game Service
  slug: game-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-game-openapi.json
- filename: evedex-billing-openapi.json
  format: json
  label: Billing Service
  slug: billing-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-billing-openapi.json
- filename: evedex-bridge-middleware-openapi.json
  format: json
  label: Bridge Middleware Service
  slug: bridge-middleware-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-bridge-middleware-openapi.json
- filename: evedex-ai-strategies-openapi.json
  format: json
  label: AI Strategies Service
  slug: ai-strategies-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-ai-strategies-openapi.json
- filename: evedex-backoffice-openapi.json
  format: json
  label: Backoffice Service
  slug: backoffice-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-backoffice-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Evedex Authentication
name_suffix: Authentication
oauth_flows: []
overview: EVEDEX secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EVEDEX
provider_slug: evedex
scheme_count: 2
schemes:
- name: AccessToken
  scheme: bearer
  sources:
  - openapi/evedex-academy-openapi.json
  - openapi/evedex-ai-strategies-openapi.json
  - openapi/evedex-auth-openapi.json
  - openapi/evedex-backoffice-openapi.json
  - openapi/evedex-billing-openapi.json
  - openapi/evedex-bridge-middleware-openapi.json
  - openapi/evedex-exchange-openapi.json
  - openapi/evedex-game-openapi.json
  - openapi/evedex-market-data-openapi.json
  - openapi/evedex-notifications-openapi.json
  - openapi/evedex-referral-openapi.json
  type: http
- in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/evedex-exchange-openapi.json
  - openapi/evedex-referral-openapi.json
  type: apiKey
slug: evedex-authentication
source_filename: evedex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/evedex-academy-openapi.json, openapi/evedex-ai-strategies-openapi.json, openapi/evedex-auth-openapi.json,\n  openapi/evedex-backoffice-openapi.json, openapi/evedex-billing-openapi.json, openapi/evedex-bridge-middleware-openapi.json,\n  openapi/evedex-exchange-openapi.json, openapi/evedex-game-openapi.json, openapi/evedex-market-data-openapi.json,\n  openapi/evedex-notifications-openapi.json, openapi/evedex-referral-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/evedex-academy-openapi.json\n  - openapi/evedex-ai-strategies-openapi.json\n  - openapi/evedex-auth-openapi.json\n  - openapi/evedex-backoffice-openapi.json\n  - openapi/evedex-billing-openapi.json\n  - openapi/evedex-bridge-middleware-openapi.json\n  - openapi/evedex-exchange-openapi.json\n  - openapi/evedex-game-openapi.json\n  - openapi/evedex-market-data-openapi.json\n\
  \  - openapi/evedex-notifications-openapi.json\n  - openapi/evedex-referral-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/evedex-exchange-openapi.json\n  - openapi/evedex-referral-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/authentication/evedex-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- cryptocurrency-exchange
- defi
- decentralized-exchange
- derivatives
- perpetual-futures
- trading
- market-data
- blockchain
- web3
- arbitrum-layer3
- fintech
---
