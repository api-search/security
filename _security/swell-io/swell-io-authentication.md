---
api_key_in:
- header
api_specs:
- filename: swell-backend-api-openapi.yml
  format: yaml
  label: Swell Backend API
  slug: swell-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/openapi/swell-backend-api-openapi.yml
- filename: swell-frontend-api-openapi.yml
  format: yaml
  label: Swell Frontend API
  slug: swell-frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/openapi/swell-frontend-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Swell Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swell secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swell
provider_slug: swell-io
scheme_count: 2
schemes:
- description: Your Swell store ID, found in the Developer section of the dashboard.
  in: header
  name: SwellStoreId
  parameter: X-Store-Id
  sources:
  - openapi/swell-backend-api-openapi.yml
  type: apiKey
- description: 'Secret API key prefixed with `sk_`. Sent as `Authorization: Basic <base64(store-id:secret-key)>` or equivalent custom header by official libraries.'
  in: header
  name: SwellSecretKey
  parameter: Authorization
  sources:
  - openapi/swell-backend-api-openapi.yml
  - openapi/swell-frontend-api-openapi.yml
  type: apiKey
slug: swell-io-authentication
source_filename: swell-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swell-backend-api-openapi.yml, openapi/swell-frontend-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SwellStoreId\n  type: apiKey\n  in: header\n  parameter: X-Store-Id\n  description: Your Swell store ID, found in the Developer section of the dashboard.\n  sources:\n  - openapi/swell-backend-api-openapi.yml\n- name: SwellSecretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Secret API key prefixed with `sk_`. Sent as `Authorization: Basic <base64(store-id:secret-key)>`\n    or equivalent custom header by official libraries.'\n  sources:\n  - openapi/swell-backend-api-openapi.yml\n  - openapi/swell-frontend-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/authentication/swell-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Commerce
- Headless Commerce
- API-First
- B2C
- B2B
- Subscriptions
- Marketplaces
- Wholesale
- Storefront
- Checkout
- Payments
- Carts
- Orders
- Catalog
- Internationalization
---
