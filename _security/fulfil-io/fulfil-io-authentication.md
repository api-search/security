---
api_key_in:
- header
api_specs:
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Sales Orders API
  slug: fulfil-io-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Products & Variants API
  slug: fulfil-io-products-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Inventory & Stock API
  slug: fulfil-io-inventory-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Customers API
  slug: fulfil-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Shipments API
  slug: fulfil-io-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Purchases API
  slug: fulfil-io-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Manufacturing API
  slug: fulfil-io-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Webhooks API
  slug: fulfil-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Model Interface API
  slug: fulfil-io-model-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fulfil Io Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fulfil secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fulfil
provider_slug: fulfil-io
scheme_count: 2
schemes:
- description: Personal access token for private integrations, sent in the X-API-KEY header. Fulfil also accepts the token via HTTP Basic authentication.
  in: header
  name: apiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/fulfil-io-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization code flow for public apps.
  flows:
  - authorizationUrl: https://{merchant_id}.fulfil.io/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{merchant_id}.fulfil.io/oauth/token
  name: oauth2
  sources:
  - openapi/fulfil-io-openapi.yml
  type: oauth2
slug: fulfil-io-authentication
source_filename: fulfil-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fulfil-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Personal access token for private integrations, sent in the X-API-KEY header.\n    Fulfil also accepts the token via HTTP Basic authentication.\n  sources:\n  - openapi/fulfil-io-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{merchant_id}.fulfil.io/oauth/authorize\n    tokenUrl: https://{merchant_id}.fulfil.io/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authorization code flow for public apps.\n  sources:\n  - openapi/fulfil-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/authentication/fulfil-io-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- ERP
- E-commerce
- Order Management
- Inventory
- Warehouse Management
- Manufacturing
- Operations
---
