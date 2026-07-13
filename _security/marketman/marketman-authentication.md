---
api_key_in:
- header
api_specs:
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Inventory & Items API
  slug: inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Vendors API
  slug: vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Purchase Orders API
  slug: purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Invoices & Docs API
  slug: invoices-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Deliveries API
  slug: deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Recipes & Menu Profitability API
  slug: recipes-menu-profitability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Marketman Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarketMan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarketMan
provider_slug: marketman
scheme_count: 1
schemes:
- description: Access token returned by GetToken, sent on every authenticated request in the AUTH_TOKEN header.
  in: header
  name: AuthToken
  parameter: AUTH_TOKEN
  sources:
  - openapi/marketman-openapi.yml
  type: apiKey
slug: marketman-authentication
source_filename: marketman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marketman-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: AUTH_TOKEN\n  description: Access token returned by GetToken, sent on every authenticated request in the\n    AUTH_TOKEN header.\n  sources:\n  - openapi/marketman-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/authentication/marketman-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Inventory
- Purchasing
- Supply Chain
- Food Service
---
