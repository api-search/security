---
api_key_in: []
api_specs:
- filename: lemonmarkets-accounts-general-api-openapi.yml
  format: yaml
  label: 'lemon.markets Accounts: General API'
  slug: lemonmarkets-accounts-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-accounts-general-api-openapi.yml
- filename: lemonmarkets-accounts-id-v-api-openapi.yml
  format: yaml
  label: 'lemon.markets Accounts: ID+V API'
  slug: lemonmarkets-accounts-id-v-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-accounts-id-v-api-openapi.yml
- filename: lemonmarkets-batch-orders-api-openapi.yml
  format: yaml
  label: lemon.markets Batch Orders API
  slug: lemonmarkets-batch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-batch-orders-api-openapi.yml
- filename: lemonmarkets-businesses-api-openapi.yml
  format: yaml
  label: lemon.markets Businesses API
  slug: lemonmarkets-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-businesses-api-openapi.yml
- filename: lemonmarkets-cash-settlement-api-openapi.yml
  format: yaml
  label: lemon.markets Cash Settlement API
  slug: lemonmarkets-cash-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-cash-settlement-api-openapi.yml
- filename: lemonmarkets-corporate-actions-api-openapi.yml
  format: yaml
  label: lemon.markets Corporate Actions API
  slug: lemonmarkets-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-corporate-actions-api-openapi.yml
- filename: lemonmarkets-documents-api-openapi.yml
  format: yaml
  label: lemon.markets Documents API
  slug: lemonmarkets-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-documents-api-openapi.yml
- filename: lemonmarkets-events-webhooks-api-openapi.yml
  format: yaml
  label: lemon.markets Events + Webhooks API
  slug: lemonmarkets-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-events-webhooks-api-openapi.yml
- filename: lemonmarkets-instruments-api-openapi.yml
  format: yaml
  label: lemon.markets Instruments API
  slug: lemonmarkets-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-instruments-api-openapi.yml
- filename: lemonmarkets-money-positions-api-openapi.yml
  format: yaml
  label: lemon.markets Money + Positions API
  slug: lemonmarkets-money-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-money-positions-api-openapi.yml
- filename: lemonmarkets-orders-api-openapi.yml
  format: yaml
  label: lemon.markets Orders API
  slug: lemonmarkets-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-orders-api-openapi.yml
- filename: lemonmarkets-persons-api-openapi.yml
  format: yaml
  label: lemon.markets Persons API
  slug: lemonmarkets-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-persons-api-openapi.yml
- filename: lemonmarkets-securities-accounts-api-openapi.yml
  format: yaml
  label: lemon.markets Securities Accounts API
  slug: lemonmarkets-securities-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-securities-accounts-api-openapi.yml
- filename: lemonmarkets-taxes-api-openapi.yml
  format: yaml
  label: lemon.markets Taxes API
  slug: lemonmarkets-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-taxes-api-openapi.yml
- filename: lemonmarkets-trades-api-openapi.yml
  format: yaml
  label: lemon.markets Trades API
  slug: lemonmarkets-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-trades-api-openapi.yml
- filename: lemonmarkets-treasury-mandates-api-openapi.yml
  format: yaml
  label: lemon.markets Treasury Mandates API
  slug: lemonmarkets-treasury-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-treasury-mandates-api-openapi.yml
- filename: lemonmarkets-workflows-api-openapi.yml
  format: yaml
  label: lemon.markets Workflows API
  slug: lemonmarkets-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemonmarkets Authentication
name_suffix: Authentication
oauth_flows: []
overview: lemon.markets secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: lemon.markets
provider_slug: lemonmarkets
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lemonmarkets-brokerage-openapi.json
  type: http
slug: lemonmarkets-authentication
source_filename: lemonmarkets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lemonmarkets-brokerage-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lemonmarkets-brokerage-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/authentication/lemonmarkets-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Brokerage
- Investing
- Trading
- Embedded Finance
- Banking as a Service
- Securities
- Wealth Management
- Germany
- Europe
---
