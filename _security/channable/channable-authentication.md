---
api_key_in:
- query
api_specs:
- filename: channable-order-connection-openapi.json
  format: json
  label: Channable Order Connection API
  slug: channable-order-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channable/refs/heads/main/openapi/channable-order-connection-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Channable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Channable secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Channable
provider_slug: channable
scheme_count: 2
schemes:
- description: 'Preferred method. Send the company API token in the Authorization header as `Authorization: Bearer [example key]`.'
  location: header
  name: BearerToken
  scheme: bearer
  sources:
  - docs
  type: http
- description: Alternative method. Send the company API token as the `access_token` query-string parameter, e.g. `?access_token=your_api_token`. The header method is recommended over query for security.
  in: query
  name: AccessTokenQuery
  parameter_name: access_token
  sources:
  - docs
  type: apiKey
slug: channable-authentication
source_filename: channable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.channable.com/api/v1/\ndocs: https://docs.channable.com/api/v1/\nsummary:\n  types: [http, apiKey]\n  api_key_in: [query]\n  http_schemes: [bearer]\n  oauth2_flows: []\n  notes: >-\n    The Channable order connection API uses a single company-level API token. It is not declared in\n    the OpenAPI securitySchemes (the components.securitySchemes object is empty); this profile is\n    sourced from the published API documentation. Only company owners can generate a token from\n    Company settings > Channable API in app.channable.com. Channable does not store tokens; generating\n    a new token automatically revokes the previous one. Rate limiting is enforced per company, so\n    minting extra tokens does not raise limits.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Preferred method. Send the company API token in the Authorization header as\n    `Authorization: Bearer [example\
  \ key]`.\n  location: header\n  sources: [docs]\n- name: AccessTokenQuery\n  type: apiKey\n  in: query\n  parameter_name: access_token\n  description: >-\n    Alternative method. Send the company API token as the `access_token` query-string parameter,\n    e.g. `?access_token=your_api_token`. The header method is recommended over query for security.\n  sources: [docs]\ntoken_lifecycle:\n  managed_at: https://app.channable.com/\n  who_can_generate: company owners only\n  storage: Channable does not store tokens; store securely on the client side\n  rotation: generating a new token immediately revokes prior tokens\n  legacy_note: >-\n    Legacy Channable API tokens were deprecated; per the changelog (November 7, 2025) legacy tokens\n    expired December 9, 2025 and integrations had to move to newly generated tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channable/refs/heads/main/authentication/channable-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Applicative Saas
- Feed Management
- Marketplaces
- E-commerce
- Product Data
- Order Management
- Advertising
- PPC
- Retail
---
