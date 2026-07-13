---
api_key_in:
- header
api_specs:
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Articles API
  slug: spod-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Orders API
  slug: spod-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Shipping API
  slug: spod-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Product Types API
  slug: spod-product-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Stock API
  slug: spod-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Subscriptions and Webhooks API
  slug: spod-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spod Authentication
name_suffix: Authentication
oauth_flows: []
overview: SPOD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SPOD
provider_slug: spod
scheme_count: 1
schemes:
- description: Per-account API access token generated in the SPOD / Spreadconnect web application. Send it as a header on every request.
  in: header
  name: access_token
  parameter: X-SPOD-ACCESS-TOKEN
  sources:
  - openapi/spod-openapi.yml
  type: apiKey
slug: spod-authentication
source_filename: spod-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spod-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: access_token\n  type: apiKey\n  in: header\n  parameter: X-SPOD-ACCESS-TOKEN\n  description: Per-account API access token generated in the SPOD / Spreadconnect web application.\n    Send it as a header on every request.\n  sources:\n  - openapi/spod-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/authentication/spod-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Print on Demand
- POD
- Dropshipping
- Fulfillment
- E-commerce
- Merchandise
- Spreadshirt
- Spreadconnect
---
