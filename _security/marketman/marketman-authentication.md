---
api_key_in:
- header
api_specs:
- filename: marketman-accounts-api-openapi.yml
  format: yaml
  label: MarketMan Accounts API
  slug: marketman-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-accounts-api-openapi.yml
- filename: marketman-authentication-api-openapi.yml
  format: yaml
  label: MarketMan Authentication API
  slug: marketman-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-authentication-api-openapi.yml
- filename: marketman-deliveries-api-openapi.yml
  format: yaml
  label: MarketMan Deliveries API
  slug: marketman-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-deliveries-api-openapi.yml
- filename: marketman-docs-api-openapi.yml
  format: yaml
  label: MarketMan Docs API
  slug: marketman-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-docs-api-openapi.yml
- filename: marketman-inventory-api-openapi.yml
  format: yaml
  label: MarketMan Inventory API
  slug: marketman-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-inventory-api-openapi.yml
- filename: marketman-items-api-openapi.yml
  format: yaml
  label: MarketMan Items API
  slug: marketman-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-items-api-openapi.yml
- filename: marketman-orders-api-openapi.yml
  format: yaml
  label: MarketMan Orders API
  slug: marketman-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-orders-api-openapi.yml
- filename: marketman-recipes-api-openapi.yml
  format: yaml
  label: MarketMan Recipes API
  slug: marketman-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-recipes-api-openapi.yml
- filename: marketman-webhooks-api-openapi.yml
  format: yaml
  label: MarketMan Webhooks API
  slug: marketman-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-webhooks-api-openapi.yml
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
