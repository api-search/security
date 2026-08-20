---
api_key_in:
- header
api_specs:
- filename: ribbon-finance-account-api-openapi.yml
  format: yaml
  label: Ribbon Finance Account API
  slug: ribbon-finance-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-account-api-openapi.yml
- filename: ribbon-finance-api-keys-api-openapi.yml
  format: yaml
  label: Ribbon Finance API Keys API
  slug: ribbon-finance-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-api-keys-api-openapi.yml
- filename: ribbon-finance-instruments-api-openapi.yml
  format: yaml
  label: Ribbon Finance Instruments API
  slug: ribbon-finance-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-instruments-api-openapi.yml
- filename: ribbon-finance-market-data-api-openapi.yml
  format: yaml
  label: Ribbon Finance Market Data API
  slug: ribbon-finance-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-market-data-api-openapi.yml
- filename: ribbon-finance-orders-api-openapi.yml
  format: yaml
  label: Ribbon Finance Orders API
  slug: ribbon-finance-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-orders-api-openapi.yml
- filename: ribbon-finance-positions-api-openapi.yml
  format: yaml
  label: Ribbon Finance Positions API
  slug: ribbon-finance-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-positions-api-openapi.yml
- filename: ribbon-finance-statistics-api-openapi.yml
  format: yaml
  label: Ribbon Finance Statistics API
  slug: ribbon-finance-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-statistics-api-openapi.yml
- filename: ribbon-finance-trade-history-api-openapi.yml
  format: yaml
  label: Ribbon Finance Trade History API
  slug: ribbon-finance-trade-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/ribbon-finance-trade-history-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ribbon Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ribbon Finance secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ribbon Finance
provider_slug: ribbon-finance
scheme_count: 2
schemes:
- description: API key obtained from Aevo account settings
  in: header
  name: AevoKey
  parameter: AEVO-KEY
  sources:
  - openapi/aevo-private-rest-api.json
  type: apiKey
- description: API secret obtained from Aevo account settings
  in: header
  name: AevoSecret
  parameter: AEVO-SECRET
  sources:
  - openapi/aevo-private-rest-api.json
  type: apiKey
slug: ribbon-finance-authentication
source_filename: ribbon-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aevo-private-rest-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AevoKey\n  type: apiKey\n  in: header\n  parameter: AEVO-KEY\n  description: API key obtained from Aevo account settings\n  sources:\n  - openapi/aevo-private-rest-api.json\n- name: AevoSecret\n  type: apiKey\n  in: header\n  parameter: AEVO-SECRET\n  description: API secret obtained from Aevo account settings\n  sources:\n  - openapi/aevo-private-rest-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/authentication/ribbon-finance-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- DeFi
- Finance
- Options
- Structured Products
- Ethereum
- Layer 2
- Vault
- Perpetuals
- Yield
---
